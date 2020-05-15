<template>
  <div id="app">
    <!-- SOURCE -->
    <div id="printMe">
      <h1>Print me!</h1>
    </div>
    <!-- OUTPUT -->
    <button @click="print">Print</button>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld
  },
  methods: {
    print() {
      // Pass the element id here
      this.$htmlToPaper("printMe");
    }
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
