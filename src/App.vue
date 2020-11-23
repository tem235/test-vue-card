<template>
  <div id="app">
    <Card/>

  </div>
</template>

<script>
import Card from "@/components/Card";

export default {
  name: 'App',
  components: {Card}
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700&display=swap');

body {
  margin: 0;
  padding: 0;
}

#app {
  font-family: 'Nunito', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #000000;
  height: 100vh;
  background-color: #f4f7fc;
  display: grid;
  align-items: center;
  justify-content: center;
}
</style>
