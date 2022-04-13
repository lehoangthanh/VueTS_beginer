<template>
  <div id="app" class="g-sidenav-show bg-gray-200">
    <!-- Leftbar -->
    <LeftBar />
    <!-- End Leftbar -->
    <main
      class="main-content position-relative max-height-vh-100 h-100 border-radius-lg"
    >
      <!-- Navbar -->
      <Header />
      <div class="container-fluid py-4">
        <router-view />
        <Footer />
      </div>
      <!-- End Navbar -->
    </main>
  </div>
</template>
<!--   Core JS Files   -->
<script src="@/assets/js/core/bootstrap.min.js"></script>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import LeftBar from "@/components/LeftBar.vue";
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";

@Component({
  components: {
    LeftBar,
    Header,
    Footer,
  },
})
export default class App extends Vue {}
</script>

<style>
@import "https://fonts.googleapis.com/css?family=Roboto:300,400,500,700,900|Roboto+Slab:400,700";
@import "https://fonts.googleapis.com/icon?family=Material+Icons+Round";
@import "./assets/css/nucleo-icons.css";
@import "./assets/css/nucleo-svg.css";
@import "./assets/css/material-dashboard.css";

/* #app {
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
} */
</style>
