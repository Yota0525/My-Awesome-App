<template>
  <nav class="navbar">
    <ul>
      <li><nuxt-link to="/">Home</nuxt-link></li>
      <li><nuxt-link to="/songs">Songs</nuxt-link></li>
      <li><nuxt-link to="/singers">Singers</nuxt-link></li>
      <li><nuxt-link to="/products">Products</nuxt-link></li>
    </ul>
  </nav>
</template>

<style scoped>
.navbar {
  background-color: #2c3e50;
  padding: 10px;
  text-align: center;
}

.navbar ul {
  list-style: none;
  padding: 0;
}

.navbar li {
  display: inline;
  margin: 0 15px;
}

.navbar a {
  color: white;
  text-decoration: none;
}
</style>
