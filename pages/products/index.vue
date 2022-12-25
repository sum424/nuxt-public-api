<template>
  <div>
    <!-- becomes /products  --> 
    <div class="grid grid-cols-4 gap -5">
      <div v-for="product in products">
        <ProductCard :product="product" />
      </div>
    </div>
    <a href="/">Go back</a>
  </div>
</template>

<script setup>
definePageMeta({
  layout: 'products'
})
// fetch products 
const {data:products } = await useFetch('https://fakestoreapi.com/products')

// 1 way of overriding default meta data 
useHead({
  title: 'Nuxt 3 Application | Merch', 
  meta: [
    {name: 'description', content: 'Nuxt 3 Merch'}
  ] 
})
</script>

<style>

</style>