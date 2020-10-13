<template>
  <div id="MapRouting">

    <layerMap> </layerMap>

  </div>
</template>

<script>

import L from "leaflet";
var  Routing = require('leaflet-routing-machine');

var layerMap = L.map('layerMap');


L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '© OpenStreetMap contributors'
}).addTo(layerMap);



L.Routing.control.hide();

L.Routing.control({
    waypoints: [
        L.latLng(57.74, 11.94),
        L.latLng(57.6792, 11.949)
    ],
    routeWhileDragging: true
}).addTo(layerMap);


export default {
  name:"MapRouting",
  components:  {
    layerMap,
  }
  
}
</script>