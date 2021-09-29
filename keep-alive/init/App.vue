<template>
  <div>
    <button @click="curTab = 'tab1'">tab1</button>
    <button @click="curTab = 'tab2'">tab2</button>
    <keep-alive>
      <component v-bind:is="curTab"></component>
    </keep-alive>
  </div>
</template>

<script>
import tab1 from "./tab1.vue";
import tab2 from "./tab2.vue";
export default {
  components: {
    tab1,
    tab2,
  },
  data() {
    return {
      curTab: "tab1",
    };
  },
};
</script>

<style>
</style>