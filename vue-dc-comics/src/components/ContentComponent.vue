<template>

    <div class="header">
        <div class="img">
            <div class="margin">
                <span id="label-series">CURRENT SERIES</span>
            </div>
        </div>
        <div class="container">

            <div class="card" v-for="(card, index) in cards" :key="index">
                <a href="#">
                    <div class="card-img">
                        <img :src="card.thumb" alt="">
                    </div>
                    <div class="card-title">
                        {{(card.series).toUpperCase()}}
                    </div>
                </a>
                
            </div>
            <button>LOAD MORE</button>
            
        </div>
    </div>
</template>

<script>


export default {
    name: 'black_content',
    props: {
        cards: Array
    }
    
}
</script>

<style scoped>
    .header {
        background-color: #1c1c1c;
    }
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 50px 0;
        color: #fff;
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: 40px 25px;
    }
    .header .img{
        height: 320px;
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;
    }
    .card {
        width: calc(100% / 6 - 21px);
        filter:brightness(0.7);

    }
    .card:hover{
        filter:brightness(1);
    }
    img{
        width: 100%;
    }
    .card-title {
        margin-top: 20px;
        font-size: 0.8rem;
    }
    .card-img {
        height: 180px;
        overflow: hidden;
    }
    button {
        text-align: center;
        background-color: #0282f9;
        color: #fff;
        border: none;
        padding: 10px 70px;
        cursor: pointer;
        font-family: 'Oswald', sans-serif;
    }
    button:hover{
        background-color: #0282f9a4;
    }
    .margin{
        max-width: 1200px;
        margin: 0 auto;
        display: flex;
        flex-grow: 1
    }
    #label-series{
        position: relative;
        top: 293px;
        text-align: center;
        font-weight: 900;
        font-size: 1.4rem;
        letter-spacing: 2px;
        background-color: #0282f9;
        color: #fff;
        padding: 10px 50px;
        font-family: 'Oswald', sans-serif;
    }
</style>