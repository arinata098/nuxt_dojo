<template>
    <div>
        <div class="grid grid-cols-4 gap-5">
            <div v-for="p in products" :key="p.id">
                <nuxt-link :to="`/products/${p.id}`">{{ p.title }}</nuxt-link>
            </div>
        </div>
    </div>
</template>

<script setup>
    // set layout untuk sub file didalam folder
    definePageMeta({
        layout: 'products'
    })

    // fetch data product
    const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>

<style scoped>
    h2 {
        margin-bottom: 20px;
        font-size: 36px;
    }
    p {
        margin: 20px 0;
    }
</style>