<template>
    <div>
        <header>
            <nav>
                <ul>
                    <nuxt-link to="/">Nuxt Dojo</nuxt-link>
                       <li> <nuxt-link to="/">Home</nuxt-link> </li>
                       <li> <nuxt-link to="/about">About</nuxt-link> </li>
                       <li> <nuxt-link to="/products">Products</nuxt-link> </li>
                </ul>
            </nav>
        </header>
        <p>Product details for {{ id }}</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde possimus eum architecto id, officiis deleniti perspiciatis dolore inventore numquam dolores.</p>
    </div>
</template>

<script setup>
    const { id } = useRoute().params
</script>

<style scoped>

</style>