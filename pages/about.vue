<template>
  <div>
    <h2>About</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Et quibusdam vel
      eaque autem aut inventore quos asperiores deserunt harum reprehenderit!
    </p>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Et quibusdam vel
      eaque autem aut inventore quos asperiores deserunt harum reprehenderit!
    </p>
    <div>{{ data }}</div>
  </div>
</template>

<script setup>
// const { data } = await useFetch('/api/ninja?name=mario', {
//   method: 'post',
//   body: {
//     age: 30,
//   },
// });
const { data } = await useFetch('/api/ninja');
</script>

<style scoped>
h2 {
  margin-bottom: 20px;
  font-size: 36px;
}
p {
  margin: 20px 0;
}
</style>
