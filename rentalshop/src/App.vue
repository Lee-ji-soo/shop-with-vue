<template>
  <div id="app">
    <header id="header">
      <b-jumbotron bg-variant="info" text-variant="white" class="rounded-0">
        <p id="header__tt">
          <strong>바로홈으로</strong> 바로구하자
        </p>
        <hr class="my-4" />
        <p>
          It uses utility classes for typography and spacing to space content out within the larger
          container.
        </p>
      </b-jumbotron>
    </header>
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <ul class="list-group">
            <li class="list-group-item active">원래대로</li>
            <li class="list-group-item">가격순</li>
            <li class="list-group-item">가나다순</li>
          </ul>
        </div>
        <div class="col-md-7">
          <div class="row">
            <div class="col-md-6">
              <img src />
              <h4>상품명</h4>
              <p>가격</p>
            </div>
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
  name: "room",
  data() {
    return {
      안녕: "hello"
    };
  },
  components: {}
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0;
}
#header__tt {
  font-size: 40px;
  font-weight: 100;
}
.list-group .list-group-item.active {
  background-color: #01cbae;
  border: none;
}
</style>
