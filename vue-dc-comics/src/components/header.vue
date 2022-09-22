<template>
    <div class="header">
        <div class="container">
            <div class="left">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="right">
                <ul>
                    <li>items</li>
                    <li>items</li>
                    <li>items</li>
                    <li>items</li>
                    <li>items</li>
                    <li>items</li>
                    <li>items</li>
                    <li>items</li>
                    <li>items</li>
                    <li>items</li>
                </ul>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
    name: 'dc_header'
}
</script>

<style scoped>
    .header {
        border-bottom: 5px solid black;
        background-color: #ffffff;
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
    }
    li {
        border-bottom: 4px solid #fff;
    }
    li:hover {
        border-color: #0282f9;
    }
    
</style>