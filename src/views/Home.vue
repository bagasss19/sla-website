<template>
  <div class="carousel carousel-slider center">

    <!-- <div class="carousel-fixed-item center">
      <a class="btn waves-effect white grey-text darken-text-2">button</a>
    </div> -->

    <div class="carousel-item green white-text" href="#one!">
      <img alt="Vue logo" src="../assets/flyer-1.jpeg" style="height:400px;width:50%;"/>
      <!-- <h2>First Panel</h2>
      <p class="white-text">This is your first panel</p> -->
    </div>
    <div class="carousel-item green white-text" href="#two!">
      <img alt="Vue logo" src="../assets/flyer-2.jpeg" style="height:400px;width:50%;"/>
      <!-- <h2>Second Panel</h2>
      <p class="white-text">This is your second panel</p> -->
    </div>
    <div class="carousel-item green white-text" href="#three!">
      <h2>Third Panel</h2>
      <p class="white-text">This is your third panel</p>
    </div>
    <div class="carousel-item blue white-text" href="#four!">
      <h2>Fourth Panel</h2>
      <p class="white-text">This is your fourth panel</p>
    </div>
  </div>

  <div class="home">
    <img alt="Vue logo" src="../assets/logo-sla.jpg" style="height:300px;width:300px;margin-top:100px;"/>
    <HelloWorld msg="Selamat Datang" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
  },
  mounted() {
    var elems = document.querySelectorAll(".carousel");
    var instances = M.Carousel.init(elems, {
      fullWidth: true,
      indicators: true,
    });
  },
};
</script>