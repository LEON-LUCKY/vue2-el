<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <MySelect @visible-change="handlerVisibleChange(arguments, '#')" />
  </div>
</template>

<script>
import MySelect from "./components/MySelect.vue";
export default {
  name: "App",
  components: {
    MySelect,
  },
  methods: {
    handlerVisibleChange(params, flag) {
      console.log(Array.from(params), flag);
    },
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
  margin-top: 60px;
}
</style>
