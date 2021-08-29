<template>
  <section class="container">
    <h3>{{ $route.params.kinds.toUpperCase() }}</h3>
  </section>
</template>

<script>
export default {
    validate(data) {
    console.log('Test validation', data.params.kinds);
    return /food/i.test(data.params.kinds);
  },
  layout: 'products',
};
</script>
