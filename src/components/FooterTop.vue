<template>
    <div>
        <ul>
            <li v-for="(link, index) in LinkFooter" :key="index" >
                <img :src="link.img" :alt="link.text">
                <p>{{link.text}}</p>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'FooterTop',
    data() {
        return{
            LinkFooter: [
                {
                    text: 'DIGITAL COMICS',
                    img: require('../assets/img/buy-comics-digital-comics.png'),
                },
                {
                    text: 'DC MERCHANDISE',
                    img: require('../assets/img/buy-comics-merchandise.png'),
                },
                {
                    text: 'SUBSCRIPTION',
                    img: require('../assets/img/buy-comics-subscriptions.png'),
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: require('../assets/img/buy-comics-shop-locator.png'),
                },
                {
                    text: 'DC POWER VISA',
                    img: require('../assets/img/buy-dc-power-visa.svg'),
                }
            ]
        }
    }
}
</script>

<style>

</style>