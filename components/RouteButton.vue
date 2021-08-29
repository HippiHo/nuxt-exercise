<template>
  <button @click="goToRoute" class="route_btn">{{text}}</button>
</template>

<script>
export default {
  name: 'RouteButton',
  props: {
    route: String,
    text: String,
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
