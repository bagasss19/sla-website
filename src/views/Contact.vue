<template>
  <div class="about">
    <h1 style="font-family: 'Bebas Neue', cursive">Kontak Kami</h1>

    <div id="mapContainer" class="basemap mapContainer"></div>
    <h4 style="font-family: 'Bebas Neue', cursive">  <i class="material-icons">location_on</i>Alamat : Graha STR, Jalan Ampera Raya Kav 11 Jakarta Selatan.</h4>
    <h4 style="font-family: 'Bebas Neue', cursive">  <img alt="ig" src="../assets/instagram.png" style="height:20px;width:20px;margin-right:10px;"/>IG: </h4>
    <h4 style="font-family: 'Bebas Neue', cursive">   <img alt="fb" src="../assets/facebook.png" style="height:20px;width:20px;margin-right:10px;"/>FB : </h4>
    <h4 style="font-family: 'Bebas Neue', cursive">   <img alt="ig" src="../assets/linkedin.png" style="height:20px;width:20px;margin-right:10px;"/>LinkedIn : </h4>
  </div>
</template>

<script>
import mapboxgl from "mapbox-gl";

export default {
  name: "Contact",
  data() {
    return {
      accessToken:
        "pk.eyJ1IjoiYWxlc2FuZHJvZ2VyYXJkIiwiYSI6ImNraG05ajdwNjA5OGYyeXFmeGp1ZHh5b3oifQ.K1CU3YqUh16FWJsLjO0h7g", // your access token. Needed if you using Mapbox maps
    };
  },
  mounted() {
    mapboxgl.accessToken = this.accessToken;

    const map = new mapboxgl.Map({
      container: "mapContainer",
      style: "mapbox://styles/mapbox/streets-v11",
      center: [106.8187796, -6.2877481],
      zoom: 12,
    });

    const nav = new mapboxgl.NavigationControl();
    map.addControl(nav, "top-right");

    const marker = new mapboxgl.Marker()
      .setLngLat([106.8187796, -6.2877481])
      .addTo(map);
  },
};
</script>

<style>
.basemap {
  width: 500px;
  height: 400px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 50px;
}
</style>