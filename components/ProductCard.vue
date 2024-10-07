<template>
    <div class="card text-center">
        <img :src="product.image" alt="product thumb" class="thumb">
        <p class="front-bold text-gray-500 m-4 truncate">{{  product.title }}</p>
        <NuxtLink :to="`products/${product.id}`">
            <p class=" font-bold mx-12 my-2 py-2 px-4 rounded bg-cyan-300 text-black bg-cyan-300">View Details</p>
        </NuxtLink>
    </div>
</template>

<script setup>
 const { product } = defineProps(['product'])
</script>

<style scoped>
.thumb {
    max-height: 120px;
    max-width: 70%;
    margin:  0 auto;
}


</style>