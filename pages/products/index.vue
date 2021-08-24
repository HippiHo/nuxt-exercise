<template>
  <div class="container">
    <h1>We offer:</h1>
    <nuxt-link to="/products/food">Food</nuxt-link>
    <span>and</span>
    <nuxt-link to="/products/drinks">Drinks</nuxt-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      productId: '',
    }
  },
  methods: {
    onLoadPoduct() {
      this.$router.push('/products/' + this.productId)
    },
  },
}
</script>
