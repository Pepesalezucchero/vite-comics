<script>
import ProductCard from './ProductCard.vue'

export default {
    name: "AppMain",
    components: {
        ProductCard,
    },
}
</script>

<template>
    <section class="container">
        <h1>CURRENT SERIES</h1>
        <ProductCard />
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.container {
    min-height: 150px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

h1 {
    color: $white;
    margin: 10px 0;
    padding: 10px 40px;
    background-color: $blue;
    font-size: 25px;
}
</style>