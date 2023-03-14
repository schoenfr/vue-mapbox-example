<script>
  import { MapboxMap, MapboxMarker } from '@studiometa/vue-mapbox-gl';
  import 'mapbox-gl/dist/mapbox-gl.css';

  export default {
    components: {
        MapboxMap, MapboxMarker
    }
  }
</script>

<template>
  <MapboxMap
    style="height: 400px"
    accessToken="pk.eyJ1IjoicnVzaGpzIiwiYSI6ImNrZ2J5cjB5bDBsb3gyenF1aWlvM3pteTIifQ.O_gv1VxHLDvC-UlG7dTYOA"
    mapStyle="mapbox://styles/mapbox/streets-v11"
    :center="[0, 0]"
    :zoom="1">
    <MapboxMarker :lng-lat="[50, 10]" />
  </MapboxMap>
</template>