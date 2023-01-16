<template>
  <h1 v-on:mousemove="getConsole()">:: HOME COMPONENT ::</h1>
  <button v-on:click="getData()">Click Here</button>
  <!-- Click Function -->
  <button v-on:dblclick="getData('Button double Click!')">Click Here</button>
  <h2>{{ count }}</h2>
</template>
<script>
export default {
  name: "HomeCompo",
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    getData() {
      this.count = this.count + 1;
    },
    getConsole() {
      console.warn("Function Called");
    },
  },
};
</script>
