<script>
</script>

<template>
    <section id="navbar-container" class="container d-flex">
        <nav>
            <span>sjbj</span>
        </nav>
        <div class="img-container">
        </div>
    </section>
</template>

<style scoped lang="scss">
#navbar-container {
    background-image: url('../../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 25rem;

    >* {
        width: 50%;
    }

    &.container {
        padding-top: 0;
        padding-bottom: 0;
    }

    .img-container {
        background-image: url('../../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        padding: 0;
    }

    nav {
        padding: 1.5rem 0;
    }
}
</style>