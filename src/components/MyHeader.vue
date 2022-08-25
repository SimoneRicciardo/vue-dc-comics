<template>

    <header class="container">
        <img src="@/assets/img/dc-logo.png" alt="">
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url" :class="link.active?'active':''" >{{link.text}}</a>
                </li>
            </ul>
        </nav>
    </header>

</template>

<script>
export default {
    name: 'MyHeader',
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    active: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    active: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    active: false
                },
                {
                    text: 'TV',
                    url: '#',
                    active: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    active: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    active: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    active: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    active: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    active: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    active: false
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">

header, ul{
    display: flex;
    justify-content: space-between;
    align-items: center;

        img{
            padding: 10px 0;
        }
}

li{
    list-style: none;

        a{
            text-decoration: none;
            margin: 0 5px;
            padding: 50px 0;
            color: black;

                &:hover {
                    border-bottom: solid 2px rgb(0, 124, 249) ;
                    color: rgb(0, 124, 249);
                        }
        }

}


</style>