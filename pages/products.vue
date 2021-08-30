<template>
  <div class="container">
    <h2>We offer:</h2>
    <nuxt-link to="/products/food">Food</nuxt-link>
    <span>and</span>
    <nuxt-link to="/products/drinks">Drinks</nuxt-link>
    <p>or</p>
    <InputField />
    <nuxt-child />
  </div>
</template>

<script>
import InputField from "~/components/InputField.vue";
export default {
  components: {
    InputField
  },
  data() {
    return {
      productId: ""
    };
  },
  methods: {
    onLoadPoduct() {
      this.$router.push("/products/" + this.productId);
    }
  },
  layout: "products"
};
</script>
