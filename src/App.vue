<template>
  <div class="container">
    <the-navbar visible></the-navbar>
    <router-view></router-view>
  </div>
</template>

<script>
import TheNavbar from "./the-navbar.vue";

export default {
  components: {
    TheNavbar,
  },
};
</script>

<style>
ul {
  all: unset;
}
li {
  all: unset;
}
a {
  all: unset;
  cursor: pointer;
}
button {
  all: unset;
}
.active {
  text-decoration: underline;
}
.container {
  display: flex;
  flex-direction: column;
  gap: 8px;
  justify-content: center;
  padding-top: 8px;
}
.card {
  background: #fff;
  width: 600px;
  margin: auto;
  padding: 8px;
  border-radius: 4px;
}
.no-padding {
  padding: 0;
}
</style>
