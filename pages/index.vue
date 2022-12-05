<template>
  <div>
    <header>
      <nav>
        <nuxt-link to="/">Nuxt Dojo</nuxt-link>
        <ul>
          <li>
            <nuxt-link to="/">Home</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/about">About</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/products">Products</nuxt-link>
          </li>
        </ul>
      </nav>
    </header>
    <h2>Home</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Et quibusdam vel
      eaque autem aut inventore quos asperiores deserunt harum reprehenderit!
    </p>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Et quibusdam vel
      eaque autem aut inventore quos asperiores deserunt harum reprehenderit!
    </p>
  </div>
</template>

<script>
export default {};
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
