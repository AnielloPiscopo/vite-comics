<script>
export default {
    name: 'MainContent',
}
</script>

<template>
    <section id="content" class="container">
        <h3 class="title">--&#62; Content goes here &#60;--</h3>
    </section>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;



#content {
    background-color: $secondary--color;

    .title {
        padding: 1.2rem 0;
    }
}
</style>