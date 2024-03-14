<template>
    <div>
        <p>Product details for {{ id }}</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde possimus eum architecto id, officiis deleniti perspiciatis dolore inventore numquam dolores.</p>
    </div>
</template>

<script setup>
    const { id } = useRoute().params

    // set layout untuk sub file didalam folder
    definePageMeta({
        layout: 'products'
    })
</script>

<style scoped>

</style>