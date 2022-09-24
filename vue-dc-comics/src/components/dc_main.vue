<template>
    <div class="main">
        <div class="container">
            <div class="content-left">
                <div class="column">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li v-for="(link, index) in elements.dc_comics" :key="index"><a href="#">{{ link }}</a></li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li v-for="(link, index) in elements.shop" :key="index"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
                <div class="column">
                    <h3>DC</h3>
                    <ul>
                        <li v-for="(link, index) in elements.dc" :key="index"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
                <div class="column">
                    <h3>SITES</h3>
                    <ul>
                        <li v-for="(link, index) in elements.sites" :key="index"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
            </div>
            <div class="content-right">
                <img src="../assets/img/dc-logo-bg.png" alt="dc-logo">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'dc_main',
    data() {
        return {
            elements: {
                dc_comics: ['Characters','Comics','Movies','TV','Games','Videos','News'],
                shop: ['Shop DC','Shop DC Collectibles'],
                dc: ['Terms Of Use','Privacy policy (New)','Ad Choises','Advertising','Jobs','Subscriptions','Talent Workshops','CPSC Certificates','Ratings','Shop Help','Contact Us'],
                sites: ['DC','MAD Magazine','DC Kids','DC Universe','DC Power Visa']
            }
        }
        
    }
}
</script>

<style scoped>
    .main {
        background-image: url('../assets/img/footer-bg.jpg');
        background-size: cover;
    }
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 15px 0;
        color: #797979;
        display: flex;
        justify-content: space-between;
    }
    h1,h2,h3,h4,h5,h6 {
        font-family: 'Oswald', sans-serif;
        color: #fff;
    }
    .content-left {
        width: calc(100% / 3);
        display: flex;
    }
    .content-right img {
        width: 80%;
        transform: translateY(-20%);
    }
    .column {
        width: calc(100% / 3);
    }
    ul {
        list-style-type: none;
        padding: 5px 0;
    }
    li {
        margin: 8px 0px;
    }
    a {
        text-decoration: none;
        color: #797979;
    }
    a:hover{
        filter: brightness(1.8);
    }
</style>