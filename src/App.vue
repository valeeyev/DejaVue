<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
  <h1>{{ title }}</h1>
  <input type="text" ref="name" />
  <button @click="mouseClick">bos uni</button>
  <!-- <HelloWorld msg="Welcome to fight club" /> -->
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  data() {
    return {
      title: "Welcome to Fight club",
    };
  },
  methods: {
    mouseClick() {
      console.log(this.$refs.name);
      this.$refs.name.classList.add("active");
      this.$refs.name.focus();
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
body {
  background: #918e8e;
}

h1 {
  display: inline-block;
  border-bottom: #2c3e50 1px solid;
  padding-bottom: 10px;
}
</style>
