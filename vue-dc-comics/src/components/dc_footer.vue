<template>
    <div class="dc_footer">
        <div class="container">
            <div class="left">
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="right">
                <span class="follow">FOLLOW US</span>
                <span>
                    <ul>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-facebook.png" alt="facebook">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-twitter.png" alt="twitter">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-youtube.png" alt="youtube">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-periscope.png" alt="periscope">
                            </a>
                        </li>
                    </ul>
                </span>
                
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'dc_footer'
}
</script>

<style scoped>
    .dc_footer{
        background-color: #303030;
        width: 100%;
    }
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 30px 0;
        color: #fff;
        display: flex;
        justify-content: space-between;
    }
    .right {
        display: flex;
    }
    .right span{
        display:flex;
        align-self: center;
    }
    ul {
        list-style-type: none;
        padding: 0;
        margin: 0 10px;
        display: flex;
        column-gap: 20px;
    }
    button {
        padding: 10px;
        background-color: transparent;
        border-color: #0282f9;
        color: #fff;
        cursor: pointer;
    }
    button:hover {
        filter:brightness(1);
        background-color: rgb(10, 10, 10);
    }
    .follow {
        margin: 0 15px;
        color: #0282f9;
    }
    a {
        filter: brightness(0.8);
    }
    a:hover {
        filter: brightness(1.8);
    }
</style>