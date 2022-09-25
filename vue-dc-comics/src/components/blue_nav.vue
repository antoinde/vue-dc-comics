<template>
    <div class="blue_nav">
        <div class="container">
            <ul>
                <li v-for="(element, index) in shop" :key="index">
                    <a href="#">
                        <div class="img-container">
                            <img :src="getImg(index)" alt="">
                        </div>

                        <div> {{ element.text }} </div>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'blue_nav',
    data() {
        return {
            shop: [
                {
                    img: 'buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS'
                },
                {
                    img: 'buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE'
                },
                {
                    img: 'buy-comics-shop-locator.png',
                    text: 'SUBSCRIPTION'
                },
                {
                    img: 'buy-comics-subscriptions.png',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    img: 'buy-dc-power-visa.png',
                    text: 'DC POWER VISA'
                }
                
            ]
        }
    },
    methods: {
        getImg(index) {
            const imageLink = '../assets/img/' + this.shop[index].img;
            console.log(imageLink);
            return imageLink;
        }
    }
    
}
</script>

<style scoped>
    .blue_nav {
        background-color: #0282f9;
    }
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 20px 0;
        color: #fff;
    }
    ul {
        display: flex;
        justify-content: space-around;
        list-style-type: none;
        column-gap: 20px;
    }
    
    li a{
        display: flex;
        align-items: center;
    }
    li:hover {
        color: black;
    }
    img {
        margin-right: 15px;
        height: 100%;
    }
    .img-container {
        height: 4rem;
    }
    
</style>