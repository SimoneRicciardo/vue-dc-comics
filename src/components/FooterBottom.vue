<template>
  <div>
    <div>
        <h2>DC COMICS</h2>
        <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
        </ul>
    </div>
    <div>
        <h2>SHOP</h2>
        <ul>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
        </ul>
    </div>
    <div>
        <h2>DC</h2>
        <ul>
            <li>terms Of Use</li>
            <li>Privacy policy (New)</li>
            <li>Ad Choices</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshops</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
        </ul>
    </div>
    <div>
        <h2>SITES</h2>
        <ul>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC Kid</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
        </ul>
    </div>
    <div>
        <div>
            <button>SIGN-UP NOW!</button>

        </div>
        <div>
            <h3>Follow us</h3>
            <ul>
                <li v-for="(link, index) in Social" :key="index">
                    <a :href="link.url"><img :src="link.logo" :alt="link.text"></a>
                </li>
            </ul>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            Social: [
                {
                    text: 'Facebook',
                    url: '#',
                    logo: require('../assets/img/footer-facebook.png'),
                },
                {
                    text: 'Twitter',
                    url: '#',
                    logo: require('../assets/img/footer-twitter.png'),
                },
                {
                    text: 'Youtube',
                    url: '#',
                    logo: require('../assets/img/footer-youtube.png'),
                },
                {
                    text: 'Pinterest',
                    url: '#',
                    logo: require('../assets/img/footer-pinterest.png'),
                },
                {
                    text: 'Periscope',
                    url: '#',
                    logo: require('../assets/img/footer-periscope.png'),
                }
            ]
        }
    }
}
</script>

<style>

</style>