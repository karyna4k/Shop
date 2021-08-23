<template>
  <li class="item">
    <img :src="product.img" :alt="product.title" />
    <h2>{{ product.title }}</h2>
  </li>
</template>

<script>
export default {
  props: {
    product: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
.item {
  width: calc((100% - 2 * 30px) / 3);
  text-align: center;
}

h2 {
  font-size: 22px;
}
</style>