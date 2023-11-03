<template>
  <div>
    <nav>
        <NuxtLink to="/">Nuxt-101</NuxtLink>
        <ul>
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
        </ul>
      </nav>
    <p>Product details for {{ id }}</p>
  </div>
</template>

<script setup>
  const { id } = useRoute().params
</script>

<style scoped>

</style>