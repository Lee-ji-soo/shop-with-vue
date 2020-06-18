<template>
  <div id="app">
    <div>
      <b-jumbotron bg-variant="info" text-variant="white" border-variant="dark">
        <template v-slot:header>BootstrapVue</template>

        <template v-slot:lead>
          This is a simple hero unit, a simple jumbotron-style component for calling extra attention to
          featured content or information.
        </template>

        <hr class="my-4" />

        <p>
          It uses utility classes for typography and spacing to space content out within the larger
          container.
        </p>
      </b-jumbotron>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-md-2">
          <ul class="list-group">
            <li class="list-group-item active" v-on:click="sortBack">원래대로</li>
            <li class="list-group-item" v-on:click="sortPrice">가격순</li>
            <li class="list-group-item">가나다순</li>
          </ul>
        </div>
        <div class="col-md-10">
          <div class="row">
            <div class="col-md-6">
              <img src />
              <h4>상품명</h4>
              <p>가격</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {}
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
