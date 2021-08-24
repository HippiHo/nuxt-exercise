<template>
  <button @click="goToRoute" class="route_btn">Find our products</button>
</template>

<script>
export default {
  name: 'RouteButton',
  props: {
    route: String,
  },
  methods: {
    goToRoute() {
      this.$router.push('/products/')
    },
  },
}
</script>

<style scoped>
.route_btn {
  padding: 10px;
  text-align: center;
  font-size: 1rem;
  font-weight: bold;
}
</style>
