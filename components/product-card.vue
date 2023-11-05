<template>
  <v-card class="py-2">
    <v-img :src="product.image" aspect-ratio="1" class="m-4"/>
    <v-card-title>{{ product.title }}</v-card-title>
    <v-card-subtitle>${{ product.price }}</v-card-subtitle>
    <v-divider></v-divider>
    <v-card-actions>
      <NuxtLink :to="`products/${product.id}`">
        <v-btn variant="flat" color="teal" class="ms-2">View Detail</v-btn>
      </NuxtLink>
    </v-card-actions>
  </v-card>
</template>

<script setup>
const { product } = defineProps(['product'])
</script>

<style lang="scss" scoped>

</style>