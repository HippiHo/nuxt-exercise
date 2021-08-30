<template>
  <section class="container">
    <h2>Welcome to the store</h2>
    <RouteButton
      :route="'/products/'"
      :text="'Find our products'"
    ></RouteButton>
  </section>
</template>

<script>
import RouteButton from "~/components/RouteButton.vue";
export default {
  components: {
    RouteButton
  }
};
</script>
