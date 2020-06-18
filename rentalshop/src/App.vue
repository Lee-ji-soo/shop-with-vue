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
    <div class="body">
      <div class="row">
        <div id="filter" class="col-md-2">
          <ul class="list-group">
            <li class="list-group-item active">원래대로</li>
            <li class="list-group-item">가격순</li>
            <li class="list-group-item">가나다순</li>
          </ul>
        </div>
        <div id="list" class="col-md-7">
          <div class="row">
            <div class="list__box col-md-6">
              <img v-bind:src="room[0].img" />
              <h5>{{room[0].title}}</h5>
              <p>{{room[0].price}}</p>
            </div>
            <div class="list__box col-md-6">
              <img v-bind:src="room[0].img" />
              <h5>{{room[0].title}}</h5>
              <p>{{room[0].price}}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Data from "./assets/data.js";

export default {
  name: "room",
  data() {
    return {
      room: Data
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

.body {
  margin: 0 50px;
}

.list-group .list-group-item.active {
  background-color: #01cbae;
  border: none;
}

#list {
  min-width: 900px;
}
#list img {
  width: 100%;
}

.row {
  justify-content: space-evenly;
}

#list .row {
  justify-content: start;
}

@media (max-width: 1140px) {
  #list {
    margin-top: 20px;
    min-width: 90%;
  }
}
</style>
