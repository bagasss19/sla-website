<template>
  <div class="navbar-fixed">
    <nav>
      <div class="nav-wrapper teal">
        <a href="#" class="brand-logo right">Logo</a>
        <a href="#" data-target="mobile-demo" class="sidenav-trigger"
          ><i class="material-icons">menu</i></a
        >
        <ul id="nav-mobile" class="left hide-on-med-and-down">
          <li><router-link to="/">Home</router-link></li>
          <li><router-link to="/about">About</router-link></li>
          <li><router-link to="/schedule">Schedule</router-link></li>
          <li><router-link to="/contact">Contact</router-link></li>
        </ul>
      </div>
    </nav>

    <!-- Buat Mobile -->
    <ul class="sidenav" id="mobile-demo">
      <li><router-link to="/">Home</router-link></li>
      <li><router-link to="/about">About</router-link></li>
      <li><router-link to="/schedule">Schedule</router-link></li>
      <li><router-link to="/contact">Contact</router-link></li>
    </ul>
  </div>
  <router-view />

  <footer class="page-footer">
    <div class="container">
      <div class="row">
        <h5 class="white-text">Supply Chain & Logistic Academy</h5>
        <p class="grey-text text-lighten-4">
          Terdepan Membangun SDM yang Handal Dalam Bidang Supply Chain &
          Logistic
        </p>
      </div>
    </div>
    <div class="footer-copyright">
      <div class="container">© 2021 Copyright Text SL Academy</div>
    </div>
  </footer>
</template>


<script>
export default {
  mounted() {
    document.addEventListener("DOMContentLoaded", function () {
      var elems = document.querySelectorAll(".sidenav");
      var instances = M.Sidenav.init(elems, options);
    });
  },
};
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

body {
  display: flex;
  min-height: 100vh;
  flex-direction: column;
}

main {
  flex: 1 0 auto;
}
</style>
