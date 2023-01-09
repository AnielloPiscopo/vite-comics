<script>
export default {
    data() {
        return {
            navItems: [
                {
                    text: 'Characters',
                    url: '#',
                    active: false,
                },

                {
                    text: 'Comics',
                    url: '#',
                    active: true,
                },

                {
                    text: 'Movies',
                    url: '#',
                    active: false,
                },

                {
                    text: 'TV',
                    url: '#',
                    active: false,
                },

                {
                    text: 'Games',
                    url: '#',
                    active: false,
                },

                {
                    text: 'Collectibles',
                    url: '#',
                    active: false,
                },

                {
                    text: 'Videos',
                    url: '#',
                    active: false,
                },

                {
                    text: 'Fans',
                    url: '#',
                    active: false,
                },

                {
                    text: 'News',
                    url: '#',
                    active: false,
                },

                {
                    text: 'Shop',
                    url: '#',
                    active: false,
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <nav class="d-flex justify-between align-center container">
            <div class="logo-container">
                <img src="../../assets/img/dc-logo.png" alt="logo" title="logo">
            </div>

            <ul class="d-flex">
                <li class="p-relative text-uppercase" :class="(navItem.active) ? 'active' : ''"
                    v-for="navItem in navItems">
                    <a :href="(navItem.url)" :alt="navItem.text">{{ navItem.text }}</a>
                    <div class="decoration p-absolute"></div>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;



header {
    background-color: $primary--color;

    .logo-container {
        width: 60px;
    }

    ul li {
        &.active {
            .decoration {
                height: 0.3rem;
                width: 60%;
                background-color: $complementary--color;

                &.p-absolute {
                    top: 50px;
                }
            }

            a {
                color: $complementary--color;
            }
        }

        a {
            margin-right: 2.3rem;
            font-size: 0.7rem;
            font-weight: bold;
            color: $darker--icon--bg-color;
        }
    }
}
</style>