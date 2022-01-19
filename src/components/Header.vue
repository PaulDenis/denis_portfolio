!<template>
    <div class="container">
        <img src="../assets/DenisPicture.jpg" alt="">
        <div class="fading">
        </div>
        <p class="text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus suscipit doloribus iusto! In, aspernatur nam impedit nulla est eaque! Rerum error dignissimos tempora voluptas nihil reiciendis itaque atque quod recusandae et fugit beatae molestiae soluta, doloremque iure minima amet pariatur mollitia dolor asperiores architecto temporibus. Labore ducimus, voluptatibus illo nulla iste quibusdam! Odit, et molestiae repudiandae aspernatur perspiciatis, aliquam voluptates obcaecati qui corrupti distinctio, eos quae nihil explicabo doloremque non sequi. Temporibus libero asperiores nostrum? Ea, voluptates iusto molestias rem repudiandae veniam nisi quia eius, officiis consequatur aliquid, magni doloremque esse eos id porro quo eveniet minus! Omnis, saepe possimus.</p>
    </div>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss" scoped>
    .container {
        width:100%;
        height: 100vh;
        position:relative;
        background-color: black;
        overflow: hidden;
        .text {
            padding-top: 100px;
            color: orangered;
            font-size: 24px;
            line-height: 40px;
        }
        img {
            height: 100vh;
            float: right;
        }
    }
    .fading{
        position: absolute;
        top: 0;
        left: 53%;
        height:100vh;
        width: 45%;

        background: rgba(0,0,0,0.9);
        background: -moz-linear-gradient(left, rgba(0,0,0,1) 0%, rgba(0,0,0,0.9) 15%, rgba(0,0,0,0) 50%, rgba(0,0,0,0.9) 85%, rgba(0,0,0,0.9) 100%);
        background: -webkit-gradient(left top, right top, color-stop(0%, rgba(0,0,0,0.9)), color-stop(15%, rgba(0,0,0,0.9)), color-stop(50%, rgba(0,0,0,0)), color-stop(85%, rgba(0,0,0,0.9)), color-stop(100%, rgba(0,0,0,0.9)));
        background: -webkit-linear-gradient(left, rgba(0,0,0,0.9) 0%, rgba(0,0,0,0.9) 15%, rgba(0,0,0,0) 50%, rgba(0,0,0,0.9) 85%, rgba(0,0,0,0.9) 100%);
        background: -o-linear-gradient(left, rgba(0,0,0,0.9) 0%, rgba(0,0,0,0.9) 15%, rgba(0,0,0,0) 50%, rgba(0,0,0,0.9) 85%, rgba(0,0,0,0.9) 100%);
        background: -ms-linear-gradient(left, rgba(0,0,0,0.9) 0%, rgba(0,0,0,0.9) 15%, rgba(0,0,0,0) 50%, rgba(0,0,0,0.9) 85%, rgba(0,0,0,0.9) 100%);
        background: linear-gradient(to right, rgba(0,0,0,1) 0%, rgba(0,0,0,0.7) 45%, rgba(0,0,0,0) 70%);
        filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#ffffff', endColorstr='#ffffff', GradientType=1 );
    }


</style>