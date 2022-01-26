!<template>
    <!-- Qui ci va la mia descrizione e una mia foto, per far vedere chi sono e qual'è il mio scopo. -->
    <div class="my_container">
        <img src="../assets/DenisPicture.jpg" alt="">
        <div class="fading">
        </div>

        <!-- testo del Header in inglese -->
        <p class="text" v-if="lingua=='american english'">
            Hi, my name is Denis Paul and I am a <span class="highlit">Web Developer</span>.
            <br>
            I started to first develope my developing skills in March of 2021, with an intensive <span class="highlit">full-stack web developer</span> course. It was not easy, but I can now create a website from scratch to afull functional website. I'm <span class="highlit">specializing</span> in Vue.JS (a framework that only makes my life a bit easyer while working). Before finding this passion a tryed out a few other paths, like <span class="highlit">Gaming development</span>. 
            In the end I fell in love with <span class="highlit">front-end developing</span> and I'm <span class="highlit">improving my skills</span> every day.
            <br>
            I also have a <span class="highlit">Youtube Channel</span> if you want to learn about programming. On this channel I do some tutorials, tips & trick, and other.
        </p>
        <h3 v-if="lingua=='american english'">If you want to know more about me and my story, <a href="#"> click here</a> <i class="fas fa-location-arrow"></i></h3>

        <!-- testo del Header in italiano -->
        <p class="text" v-if="lingua=='italian'">
            Ciao, mi chiamo Denis Paul e sono un <span class="highlit">Web Developer</span>.
            <br>
            Ho iniziato a svillupare le mie abilità a Marzo del 2021, con un corso intensivo da <span class="highlit">full-stack web developer</span>. Non è stato facile, ma adesso posso creare un sito completo da 0. Mi sto <span class="highlit">specializzando</span> in Vue.JS (un framework che mi rende la vita più facile mentre lavoro). Prima di trovare questa passione ho provato altre strade, come lo <span class="highlit">sviluppatore di videogiochi</span>. 
            Alla fine mi sono innamorato dello <span class="highlit">sviluppo front-end</span> e sto <span class="highlit">migliorando le mie abilità</span> ogni giorno.
            <br>
            Ho anche un <span class="highlit">canale YouTube</span> se volete imparare a programmare. Su questo canale faccio dei tutorial, do consigli, trucchi e altri tipi di contenuti.
        </p>
        <h3 v-if="lingua=='italian'">Se vuoi sapere di più su di me e la mia storia, <a href="#"> clicca qui</a> <i class="fas fa-location-arrow"></i></h3>

        <!-- testo del Header in rumeno -->
        <p class="text" v-if="lingua=='romanian'">
            Salut, ma numesc Denis Paul si sunt un <span class="highlit">Web Developer</span>.
            <br>
            Am inceput sa imi cladesc abilitatile in Martie din 2021, cu un curs intensiv ca <span class="highlit">full-stack web developer</span>. Nu a fost usor, dar acuma pot sa creez un website complet de la 0. Ma <span class="highlit">specializez</span> in Vue.JS (un framework care imi face viata mai usoara cand lucrez). Inainte de a gasii aceasta pasiune am incercat alte strazi, cum ar fi <span class="highlit">programator de jocuri video</span>. 
            Pana la urma m-am indragostit de <span class="highlit">programarea front-end</span> si <span class="highlit">imi imbunatatesc abilitatiile</span> in fie care zi.
            <br>
            Am si un <span class="highlit">canal YouTube</span> daca vreti sa invatati sa programati. Pe acest canal fac tutoriale, dau sfaturi si 'trucuri' impreuna cu alte continuturii.
        </p>
        <h3 v-if="lingua=='romanian'">Daca vrei sa afli mai multe despre mine, <a href="#"> apasa aici</a> <i class="fas fa-location-arrow"></i></h3>
    </div>
</template>

<script>
export default {
    name: 'Header',
    props: {
        lingua: String
    }
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
        // overflow: hidden;
        .text {
            padding-top: 100px;
            width: 51%;
            color: $main_color;
            font-size: 22px;
            line-height: 40px;
        }
        h3 {
            font-size: 24px;
                margin-top: 50px;
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
</style>