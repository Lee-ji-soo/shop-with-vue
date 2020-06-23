<template>
<div id="app">
  <header>
    <Navibar />
    <div id="main">
      <b-jumbotron bg-variant="info" text-variant="white" class="rounded-0">
        <p id="title">
          <strong>바로홈으로</strong> 바로구하자
        </p>
        <hr class="my-4" />
        <p>
          It uses utility classes for typography and spacing to space content out within the larger
          container.
        </p>
      </b-jumbotron>
    </div>
  </header>
  <body>
    <div id="wrap">
      <div id="filter">
        <ul class="list-group">
          <li class="list-group-item active">원래대로</li>
          <li class="list-group-item">가격순</li>
          <li class="list-group-item">가나다순</li>
        </ul>
      </div>
      <div id="products">
        <Products v-for="(room,i) in rooms" v-bind:key="i" v-bind:room="rooms[i]"></Products>
      </div>
    </div>
  </body>
  <Footer />
</div>
</template>

<script>
import Data from "./assets/data.js";
import Products from "./components/Products.vue";
import Navibar from "./components/Navibar.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "room",
  data() {
    return {
      rooms: Data
    };
  },
  components: {
    Products,
    Navibar,
    Footer
  }
};
</script>

<style>
@import "./assets/css/index.css";
@import "./assets/css/reset.css";

* {
  margin: 0px;
  padding: 0px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 0;
}
</style>
