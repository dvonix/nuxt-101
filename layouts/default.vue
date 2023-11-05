<template>
  <v-app>
    <header class="shadow-sm bg-white">
      <nav class="container py-4 px-12 flex justify-between">
      <NuxtLink to="/" class="font-bold">Nuxt-101</NuxtLink>
      <ul class="flex gap-4">
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/products" class="btn">Products</NuxtLink></li>
      </ul>
    </nav>
    </header>
    
    <div class="container py-4 px-12">
      <slot/>
    </div>
  </v-app>

</template>

<style scoped>
  .router-link-exact-active {
    color: #12b488;
  }
</style>