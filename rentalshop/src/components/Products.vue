<template>
  <div class="list__box">
    <img v-bind:src="room.img" />
    <h5>{{room.title}}</h5>
    <p>{{room.price}}</p>
  </div>
</template>

<script>
export default {
  props: {
    room: Object
  }
};
</script>
