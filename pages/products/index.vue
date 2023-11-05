<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="product in products">
        <product-card :product="product"/>
      </div>
    </div>
  </div>
</template>

<script setup>
  definePageMeta({
    layout: 'products'
  })

  const url = "https://fakestoreapi.com/products"
  const { data: products } = await useFetch(url)
</script>

<style scoped>

</style>