<script setup lang="ts">
const { product } = defineProps(['product'])
</script>

<template>
  <v-container class="bg-white rounded">
    <v-row no-gutters>
      <v-col cols="12" sm="6">
        <v-img :src="product.image" aspect-ratio="1" class="m-4"/>
      </v-col>
      <v-col cols="12" sm="6">
        <p class="text-h3 mb-8">{{ product.title }}</p>
        <p class="text-subtitle-1 mb-4">Price - ${{ product.price }}</p>
        <v-divider></v-divider>
        <p>{{ product.description }}</p>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>

</style>