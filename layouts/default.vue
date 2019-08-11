<template>
  <div>
    <Header></Header>
    <nuxt />
  </div>
</template>

<script>
import Header from "~/components/Header.vue";
export default {
  components: {
    Header
  }
};
</script>
<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
html {
  font-size: 40px;
  font-family: "Raleway", sans-serif;
}
body {
  margin: 0;
}
</style>
