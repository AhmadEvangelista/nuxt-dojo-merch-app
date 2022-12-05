<template>
  <div>
    <ProductDetails :product="products" />
  </div>
</template>

<script setup>
const { id } = useRoute().params;
const uri = `https://fakestoreapi.com/products/${id}`;

const { data: products } = await useFetch(uri, { key: id });

definePageMeta({
  layout: 'products',
});
</script>

<style scoped></style>
