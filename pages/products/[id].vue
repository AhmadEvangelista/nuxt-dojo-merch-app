<template>
  <div>
    <Head>
      <Title>Nuxt Dojo | {{ products.title }}</Title>
      <Meta name="description" :content="products.description"></Meta>
    </Head>
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
