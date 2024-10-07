<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container-mx-auto p-4 flex justify-between bg-red-50">
                <h1>Products List</h1>
                <ul  class="flex gap-4">
                    <li>
                        <NuxtLink to="/" class="btn">Landing Page</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/slice-simulator" class="btn">Simulation Page</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/products" class="btn">Products Page</NuxtLink>
                    </li>
                </ul>
            </nav>
        </header>

        <div  class="container mx-auto p-4">
            <slot />
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>
.router-link-exact-active {
    @apply font-bold py-2 px-4 rounded bg-cyan-300 text-black bg-cyan-300;
}</style>