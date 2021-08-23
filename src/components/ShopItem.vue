<template>
  <li class="item">
    <img :src="product.img" :alt="product.title" />
    <router-link :to="/shop/ + product.id" class="link">{{ product.title }}</router-link>
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
</style>