!<template>
    <!-- Qui ci va la mia descrizione e una mia foto, per far vedere chi sono e qual'è il mio scopo. -->
    <div class="my_container">
        <img src="../assets/DenisPicture.jpg" alt="">
        <div class="fading">
        </div>
        <p class="text">
            Hi, my name is Denis Paul and I am a <span>Web Developer</span>.
            <br>
            I started to first develope my developing skills in March of 2021, with an intensive <span>full-stack web developer</span> course. It was not easy, but I can now create a website from scratch to afull functional website. I'm <span>specializing myself</span> in Vue.JS (a framework that only makes my life a bit easyer while working). Before finding this passion a tryed out a few other paths, like <span>Gaming development</span>. 
            In the end I fell in love with <span>front-end developing</span> and I'm <span>improving my skills</span> every day.
            <br>
            I also have a <span>Youtube Channel</span> if you want to learn about programming. On this channel I do some tutorials, tips & trick, and other.
        </p>
        <h3>If you want to know more about me and my story, <a href="#"> click here</a> <i class="fas fa-location-arrow"></i></h3>
    </div>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';

    .my_container {
        width:100%;
        height: 100vh;
        padding-left: 20px;
        position:relative;
        background-color: black;
        overflow: hidden;
        .text {
            padding-top: 100px;
            color: $main_color;
            font-size: 22px;
            line-height: 40px;
            span {
                color: white;
            }
        }
        h3 {
                margin-top: 100px;
                color: $opposite_color;
                a {
                    color: $opposite_color;
                }
                a:hover {
                    cursor: pointer;
                }
            }
        img {
            height: 100vh;
            float: right;
        }
    }
    .fa-location-arrow {
        position: relative;
        top: 20px;
        right: 10px;
        transform: rotate(270deg);
        animation: click_anim 4s infinite;
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

    @keyframes click_anim {
        0% {
            top: 20px;
            right: 10px;
        }
        50% {
            top: 40px;
            right: -20px;
        }
        100% {
            top: 20px;
            right: 10px;
        }
    }
</style>