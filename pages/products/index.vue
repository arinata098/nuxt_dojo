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
        <h2>Products</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit ad aperiam omnis placeat ducimus laudantium quisquam, repellendus ratione eum eveniet.</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit ad aperiam omnis placeat ducimus laudantium quisquam, repellendus ratione eum eveniet.</p>
    </div>
</template>

<script setup>

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