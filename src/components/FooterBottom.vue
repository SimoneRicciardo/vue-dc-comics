<template>
    <div>
        <div class="back_footer_link">
            <div class="my_container containet_list_style">
                <div class="style_list">
                    <div>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="(link, index) in linkDcComics" :key="index">
                                <a :href="link.url">{{link.text}}</a>
                            </li>
                        </ul>
                        <h3>SHOP</h3>
                        <ul>
                            <li v-for="(link, index) in LinkShop" :key="index">
                                <a :href="link.url">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h3>DC</h3>
                        <ul>
                            <li v-for="(link, index) in linkDc" :key="index">
                                <a :href="link.url">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h3>SITES</h3>
                        <ul>
                            <li v-for="(link, index) in linkSites" :key="index">
                                <a :href="link.url">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="img_jumbo_footer">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <div class="link_social_bar">
            <div class="my_container link_social">
                <div>
                    <button>SIGN-UP NOW!</button>
                </div>
                <div>
                    <ul class="icon_link">
                        <h3>Follow us</h3>
                        <li v-for="(link, index) in Social" :key="index">
                            <span class="flex_social">
                                <a :href="link.url"><img :src="link.logo" :alt="link.text"></a>
                            </span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {

            linkDcComics: [
                {
                    text: 'Characters',
                    url: '#',
                },
                {
                    text: 'Comics',
                    url: '#',
                },
                {
                    text: 'Movies',
                    url: '#',
                },
                {
                    text: 'TV',
                    url: '#',
                },
                {
                    text: 'Games',
                    url: '#',
                },
                {
                    text: 'Videos',
                    url: '#',
                },
                {
                    text: 'News',
                    url: '#',
                }
            ],

            LinkShop: [
                {
                    text: 'Shop DC',
                    url: '#',
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#',
                }
            ],

            linkDc: [
                {
                    text: 'terms Of Use',
                    url: '#',
                },
                {
                    text: 'Privacy policy (New)',
                    url: '#',
                },
                {
                    text: 'Ad Choices',
                    url: '#',
                },
                {
                    text: 'Advertising',
                    url: '#',
                },
                {
                    text: 'Jobs',
                    url: '#',
                },
                {
                    text: 'Subscriptions',
                    url: '#',
                },
                {
                    text: 'Talent Workshops',
                    url: '#',
                },
                {
                    text: 'CPSC Certificates',
                    url: '#',
                },
                {
                    text: 'Ratings',
                    url: '#',
                },
                {
                    text: 'Shop Help',
                    url: '#',
                },
                {
                    text: 'Contact Us',
                    url: '#',
                }
            ],

            linkSites: [
                {
                    text: 'DC',
                    url: '#',
                },
                {
                    text: 'MAD Magazine',
                    url: '#',
                },
                {
                    text: 'DC Kid',
                    url: '#',
                },
                {
                    text: 'DC Universe',
                    url: '#',
                },
                {
                    text: 'DC Power Visa',
                    url: '#',
                }
            ],

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

<style scoped lang="scss">

.back_footer_link{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;

        h3{
            color: white;
        }

}

ul{
    padding: 20px 0;

        li{
            list-style: none;

                a{
                    text-decoration: none;
                    color: rgb(112, 111, 110);
                }
        }
}

.style_list{
    display: flex;

}
.img_jumbo_footer{
    translate: 0px -110px;
} 

.containet_list_style{
    display: flex;
    justify-content: space-between;
    padding: 35px 0;
}

.link_social_bar{
    background-color: rgb(48, 48, 48);
}

.link_social{
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-direction: row;
}

.icon_link{
    display: flex;
    align-items: center;

        h3{
            color: rgb(8, 128, 252);
        }

        li{
            padding: 5px;
        }
}

</style>