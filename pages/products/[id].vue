<template>
    <div>
        <!-- <p>Product details for {{ id }}</p>
        <h1 class="font-bold">{{ product.title }}</h1>
        <p> $.{{ product.price }}</p>
        <p>{{ product.description }}</p> -->
        <ProductDetails :product="product" />
    </div>
</template>

<script setup>
    const { id } = useRoute().params
    const uri = 'https://fakestoreapi.com/products/' + id;

    const { data: product } = await useFetch(uri, { key: id})

    if (!product.value) {
        throw createError({ statusCode: 404, statusMessage: 'Product not found', fatal: true})
    }

    // set layout untuk sub file didalam folder
    definePageMeta({
        layout: 'products'
    })

</script>

<style scoped>

</style>