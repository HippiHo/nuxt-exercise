<template>
  <div class="container">
    <h2>We offer:</h2>
    <nuxt-link to="/products/food">Food</nuxt-link>
    <span>and</span>
    <nuxt-link to="/products/drinks">Drinks</nuxt-link>
    <nuxt-child />
  </div>
</template>

<script>
export default {
  data() {
    return {
      productId: "",
    };
  },
  methods: {
    onLoadPoduct() {
      this.$router.push("/products/" + this.productId);
    },
  },
  layout: 'products'
};
</script>