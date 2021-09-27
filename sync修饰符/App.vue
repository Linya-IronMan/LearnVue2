<template>
  <div id="app">
    <sync :count.sync="data"></sync>
    app:data= {{data}}
    <button @click="data++">plus</button>
  </div>
</template>

<script>
import sync from "./sync.vue";
export default {
  components: {
    sync,
  },
  data() {
    return {
      data: 0,
    };
  },
};
</script>


