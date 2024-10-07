<template>
    <div class="grid grid-cols-3 gap-8">
    <div v-for="p in products">
        <ProductCard :product="p" />
    </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: 'products'
})

// Fetch the products
const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>

<style scoped>

</style>