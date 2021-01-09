<template>
  <div class="hello">
    <!-- <h1 style="font-family: 'Bebas Neue', cursive;">{{ msg }}</h1> -->
    <h4 style="font-family: 'Bebas Neue', cursive">
      Selamat Datang di Website Resmi Supply Chain and Logistic Academy
    </h4>

    <div class="row">
      <div class="col s12 m4">
        <div class="card">
          <div class="card-image">
             <i class="large material-icons">people</i>
            <h4>Terbatas</h4>
          </div>
          <div class="card-content">
            <p>
              Kuota Peserta dibatasi 50 orang
            </p>
          </div>
        </div>  
      </div>

      <div class="col s12 m4">
        <div class="card">
          <div class="card-image">
             <i class="large material-icons">money_off</i>
            <h4>Gratis</h4>
          </div>
          <div class="card-content">
            <p>
              Nikmati Pelatihan Senilai Rp 40 Juta Secara Gratis
            </p>
          </div>
        </div>  
      </div>

      <div class="col s12 m4">
        <div class="card" style="height:239px;">
          <div class="card-image">
             <i class="large material-icons">stars</i>
            <h4>Berkualitas</h4>
          </div>
          <div class="card-content">
            <p>
              Dihadiri Puluhan Praktisi dan Akademisi yang Sudah Ahli Sebagai Narasumber
            </p>
          </div>
        </div>  
      </div>
    </div>

    <router-link to="/schedule"
      ><a class="waves-effect waves-light btn" style="margin-bottom: 100px"
        ><i class="material-icons left">date_range</i>Lihat Jadwal</a
      ></router-link
    >
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap");

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
/* a {
  color: #42b983;
} */
</style>