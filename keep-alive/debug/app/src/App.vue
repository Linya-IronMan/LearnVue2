<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <button @click="curTab = 'tab1'">tab1</button>
    <button @click="curTab = 'tab2'">tab2</button>
    <keep-alive>
      <component :is="curTab"></component>
    </keep-alive>
  </div>
</template>

<script>
import tab1 from "./components/tab1.vue"
import tab2 from "./components/tab2.vue"

export default {
  name: 'App',
  components: {
    tab1,
    tab2,
  },
  data() {
    return {
      curTab: "tab1"
    }
  }
}
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
