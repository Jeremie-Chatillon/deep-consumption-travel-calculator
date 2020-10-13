<template>
  <div>
    <h3>MapRoutingBase</h3>
    <div id="MapRoutingBase"></div>
    <el-button>Default</el-button>1
      <el-row>
        <el-col :span="12"><div class="grid-content bg-purple">a</div></el-col>
        <el-col :span="12"><div class="grid-content bg-purple-light">b</div
        ></el-col>
      </el-row>
  </div>
</template>

<script>
import "leaflet/dist/leaflet.css";
import L from "leaflet";

import { Col, Row, Button } from 'element-ui';

require("leaflet-routing-machine");
delete L.Icon.Default.prototype._getIconUrl;

L.Icon.Default.mergeOptions({
  iconRetinaUrl: require("leaflet/dist/images/marker-icon-2x.png"),
  iconUrl: require("leaflet/dist/images/marker-icon.png"),
  shadowUrl: require("leaflet/dist/images/marker-shadow.png"),
});

console.info("r", L.Routing);
console.info("L", L);

export default {
  name: "MapRoutingBase",
  components: {
    [Col.name]: Col,
    [Row.name]: Row,
    [Button.name]: Button,
  },
  data() {
    return {
      map: null,
    };
  },
  mounted() {
    this.map = L.map("MapRoutingBase").setView([51.959, -8.623], 12);
    L.tileLayer("http://{s}.tile.osm.org/{z}/{x}/{y}.png", {
      attribution:
        '&copy; <a href="http://osm.org/copyright">OpenStreetMap</a> contributors',
    }).addTo(this.map);

    var routing = L.Routing.control({
      waypoints: [
        L.latLng(57.74, 11.94),
        L.latLng(57.6792, 11.949),
        L.latLng(57.6792, 11.91),
      ],
      routeWhileDragging: true,
    }).addTo(this.map);

    // Hide routing container
    routing._container.style.display = "None";
  },
  beforeDestroy() {
    if (this.map) {
      this.map.remove();
    }
  },
};
</script>

<style scoped>
#MapRoutingBase {
  width: 100%;
  height: 300px;
}
.el-row {
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .el-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
</style>