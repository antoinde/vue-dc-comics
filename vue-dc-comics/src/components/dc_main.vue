<template>
    <div class="main">
        <div class="container">
            <div class="content-left">
                <div class="column">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li>items</li>
                        <li>items</li>
                    </ul>
                </div>
                <div class="column">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                    </ul>
                </div>
                <div class="column">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                        <li>items</li>
                    </ul>
                </div>
            </div>
            <div class="content-right">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'dc_main'
}
</script>

<style scoped>
    .main {
        background-image: url('../assets/img/footer-bg.jpg');
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
        color: #fff;
    }
    .content-left {
        width: calc(100% / 3);
        display: flex;
    }
    .content-right img {
        position: relative;
        width: 90%;
        top: -70px;
    }
    .column {
        width: calc(100% / 3);
    }
    ul {
        list-style-type: none;
        padding: 5px 0;
    }
</style>