<script>
</script>

<template>
    <header>
        <nav class="d-flex justify-between align-center container">
            <div class="logo-container">
                <img src="../../assets/img/dc-logo.png" alt="">
            </div>

            <ul class="d-flex">
                <li class="p-relative">
                    <a href="#">sha</a>
                    <div class="decoration p-absolute"></div>
                </li>

                <li class="p-relative active">
                    <a href="#">sha</a>
                    <div class="decoration p-absolute"></div>
                </li>

                <li class="p-relative">
                    <a href="#">sha</a>
                    <div class="decoration p-absolute"></div>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped lang="scss">
.logo-container {
    width: 7%;
}

ul li {
    margin-right: 2.3rem;

    &.active {
        .decoration {
            height: 0.3rem;
            width: 100%;

            &.p-absolute {
                top: 67px;
            }
        }
    }
}
</style>