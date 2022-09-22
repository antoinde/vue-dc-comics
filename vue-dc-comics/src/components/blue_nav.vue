<template>
    <div class="blue_nav">
        <div class="container">
            <ul>
                <li><span>logo </span><span>item</span></li>
                <li><span>logo </span><span>item</span></li>
                <li><span>logo </span><span>item</span></li>
                <li><span>logo </span><span>item</span></li>
                <li><span>logo </span><span>item</span></li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'blue_nav'
}
</script>

<style scoped>
    .blue_nav {
        background-color: #0282f9;
    }
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 15px 0;
        color: #fff;
    }
    ul {
        display: flex;
        justify-content: space-around;
        list-style-type: none;
    }
    
</style>