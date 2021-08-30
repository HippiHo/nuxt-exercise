<template>
  <div>
    <input type="text" v-model="searchText" />
    <RouteButton
      :route="`/products/${searchText}`"
      :text="'Search'"
    ></RouteButton>
  </div>
</template>

<script>
import RouteButton from "~/components/RouteButton.vue";
export default {
  name: "InputField",
  components: {
    RouteButton
  },
  props: {
    inputId: String
  },
  data() {
    return {
      searchText: ""
    };
  }
};
</script>

<style scoped>
input {
  max-width: 100%;
  padding: 10px;
}
</style>
