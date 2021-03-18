<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld :msg="message" @messageChanged="edit($event)" />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
  data() {
    return {
      message: "Welcome to Your Vue.js App",
    };
  },
  methods: {
    edit($event) {
      this.message = $event;
    },
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
