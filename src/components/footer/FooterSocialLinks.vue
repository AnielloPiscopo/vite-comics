<script>
export default {
    data() {
        return {
            path: 'src/assets/img/footer-',
            socialLinks: [
                {
                    url: 'facebook',
                    description: 'Facebook',
                },


                {
                    url: 'twitter',
                    description: 'Twitter',
                },


                {
                    url: 'youtube',
                    description: 'Youtube',
                },


                {
                    url: 'pinterest',
                    description: 'Pinterest',
                },


                {
                    url: 'periscope',
                    description: 'Google Maps',
                },
            ]
        }
    }
}
</script>

<template>
    <section id="social-links" class="container d-flex justify-between">
        <a href="" class="btn text-uppercase d-flex align-center">Sign-Up Now!</a>
        <div class="social-links-container d-flex align-center">
            <span class="text-uppercase">Follow Us</span>
            <ul class="d-flex">
                <li v-for="socialLink in socialLinks"><a href="#"><img :src="path + socialLink.url + '.png'"
                            :alt="socialLink.description + '\'s icon'" :title="socialLink.description + '\'s icon'"></a>
                </li>
            </ul>
        </div>
    </section>
</template>

<style scoped lang="scss">
ul li {
    margin-left: 1rem;
}

span {
    font-weight: bold;
}

.btn {
    padding: 0.5rem;
}
</style>