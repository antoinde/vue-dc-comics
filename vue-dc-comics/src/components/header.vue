<template>
    <div class="header">
        <div class="container">
            <div class="left">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="right">
                <ul>
                    <li v-for="(link, index) in links" :key="index">
                        <a href="#"> {{link}} </a>
                    </li>
                </ul>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
    name: 'dc_header',
    data() { //lo uso nel componente stesso
        return {
         links: ['CHARACTERS','COMICS','MOVIES', 'TV', 'GAMES','COLLECTIBLES','VIDEOS','FANS','NEWS', 'SHOP']
        }
    }
}
</script>

<style scoped>
    .header {
        background-color: #ffffff;
        font-family: 'Oswald', sans-serif;
        font-size: 0.85rem;
        font-weight: 900;
    }
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 10px 0;
        display: flex;
        justify-content: space-between;
    }
    .left {
        margin: auto 0;
    }
    .left img{
        width: 3rem;
    }
    ul {
        display: flex;
        list-style-type: none;
        column-gap: 1.5rem;
        height: 85%;
    }
    li {
        border-bottom: 4px solid #fff;
    }
    li:hover {
        border-color: #0282f9;
        transform: scale(120%);
    }
    a{
        color: black;
    }
</style>