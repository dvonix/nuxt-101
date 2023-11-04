<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container py-4 px-12">
        <NuxtLink to="/products" class="font-bold">Nuxt-101 Store</NuxtLink>
      </nav>
    </header>
    
    <div class="container mx-auto py-4 p-12">
      <slot/>
    </div>

    <footer class="container mx-auto py-4 px-12 flex justify-between border-t-2">
      <ul class="flex gap-4">
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/products">Products</NuxtLink></li>
      </ul>
    </footer>
  </div>
</template>

<style scoped>
  .router-link-exact-active {
    color: #12b488;
  }
</style>