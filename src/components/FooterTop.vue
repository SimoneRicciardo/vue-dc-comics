<template>
    <div class="mystyle">
        <ul class="container">
            <li v-for="(link, index) in LinkFooter" :key="index" >
                <a :href="link.url">
                    <img :src="link.img" :alt="link.text">
                    <p>{{link.text}}</p>
                </a>
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
                    url:'#'
                },
                {
                    text: 'DC MERCHANDISE',
                    img: require('../assets/img/buy-comics-merchandise.png'),
                    url:'#'
                },
                {
                    text: 'SUBSCRIPTION',
                    img: require('../assets/img/buy-comics-subscriptions.png'),
                    url:'#'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: require('../assets/img/buy-comics-shop-locator.png'),
                    url:'#'
                },
                {
                    text: 'DC POWER VISA',
                    img: require('../assets/img/buy-dc-power-visa.svg'),
                    url:'#'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">

.mystyle{
    background-color: rgb(2, 130, 249);
}

ul{
    display: flex;
    justify-content: space-around;
    padding: 20px 0;

        li{
            list-style: none;
            z-index: 999;

                a{
                    display: flex;
                    align-items: center;
                    text-decoration: none;
                    color: white;

                        img{
                            width: 65px;
                            height: 65px;
                            padding: 10px 15px;
                        }
                }
        }
}

</style>