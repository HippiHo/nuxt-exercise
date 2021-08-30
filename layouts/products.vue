<template>
  <div>
    <Header />
    <h1>THE PRODUCTS</h1>
    <Nuxt />
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
*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

html {
  background-color: #b6ff7b;
}
</style>
