<script>
export default {
    name: "AppMain"
}
</script>

<template>
    <section class="container">
        <h1>Content goes here</h1>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables' as *;

.container {
    min-height: 150px;
    display: flex;
    align-items: center;
}
h1 {
    font-size: 30px;
    color: $white;
}

</style>