<template>
  <div>
    <ProductDetails :product="products" />
  </div>
</template>

<script setup>
const { id } = useRoute().params;
const uri = `https://fakestoreapi.com/products/${id}`;

const { data: products } = await useFetch(uri, { key: id });

if (!products.value) {
  throw createError({
    statusCode: 404,
    statusMessage: 'Product not found',
    fatal: true,
  });
}

definePageMeta({
  layout: 'products',
});
</script>

<style scoped></style>
