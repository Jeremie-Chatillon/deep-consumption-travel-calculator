<template>
  <div id="app">
    Hello App

    <Map />
    <map-routing-base></map-routing-base>1
    <div >
      <!--<MapRouting />
  <MapRoutingBase />
  -->
    </div>
  </div>
</template>

<script>
import Map from "./components/map/Map.vue";
//import MapRouting from "./components/map/MapRouting.vue";
import MapRoutingBase from "./components/map/MapRoutingBase.vue";

export default {
  name: 'App',
  components: {
    Map,
    //MapRouting,
    MapRoutingBase,
  },
  data() {
    return {
      display: false,
    };
  },
};
</script>

<style>

@import "/node_modules/leaflet/dist/leaflet.css";

#mapContainer {
  width: 100%;
  height: 100%;
}
</style>
