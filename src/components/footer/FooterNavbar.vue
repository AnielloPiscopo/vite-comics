<script>
export default {
    data() {
        return {
            navSections: [
                {
                    title: 'Dc Comics',
                    navItems: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News',
                    ]
                },

                {
                    title: 'Shop',
                    navItems: [
                        'Shop DC',
                        'Shop DC Collectibles',
                    ]
                },

                {
                    title: 'DC',
                    navItems: [
                        'Terms of Use',
                        'Privacy policy(new)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us',
                    ]
                },

                {
                    title: 'Sites',
                    navItems: [
                        'DC',
                        'MAD Magazines',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa',
                    ]
                },
            ]
        }
    }
}
</script>

<template>
    <section id="navbar-container" class="container d-flex">
        <nav class="d-flex wrap column">
            <div class="nav-item" v-for="navSection in navSections">
                <h3 class="text-uppercase">{{ navSection.title }}</h3>
                <ul>
                    <li v-for="navItem in navSection.navItems"><a href="#">{{ navItem }}</a></li>
                </ul>
            </div>
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

        .nav-item {
            margin: 1rem 0;

            h3 {
                padding-bottom: 0.7rem;
            }

            li {
                font-size: 0.7rem;
                padding-bottom: 0.2rem;
            }
        }
    }
}
</style>