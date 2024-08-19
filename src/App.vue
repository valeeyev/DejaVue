<template>
  <h1>{{ title }}</h1>
  <modal></modal>
</template>

<script>
import modal from "./components/Modal.vue";
export default {
  name: "App",
  components: { modal },
  data() {
    return {
      title: "Welcome to CSedu",
    };
  },
  methods: {},
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
body {
  background: #918e8e;
}

h1 {
  display: inline-block;
  border-bottom: #2c3e50 1px solid;
  padding-bottom: 10px;
}
</style>
