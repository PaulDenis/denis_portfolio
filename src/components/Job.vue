<template>
    <div class="job_desc">

        <!-- Testo inglese -->
        <div v-if="lingua=='american english'">
            <img src="../assets/DenixLogo.png" alt="Fox logo" class="logo">
            <p class="upper">With my Freelancing career I want to offer <span class="highlit">good quality service</span>, at a fair price since I am still learning. I won't start my activity until I am not confident enough that <span class="highlit">I can create almost anything</span> my client will ask for. During my experience I will <span class="highlit">create some pre-sets</span> for the clients to choose from, in case they want a cheaper website. The presets will be less personalizable, but also a starting point for a completly personalized website. </p>
            <p class="lower">Keep in mind that, even if I' am a full stack, for now I am a <span class="highlit">front-end oriented</span> developer. That means that for now I am improving my front-end skills more than the back-end skills. So if you want a website with a database, it will take <span class="highlit">more time</span> for me to complete it, but I can still do it. In the future I will complete my knowlege with back-end services too.</p>
            <h3>To read more about my plan, <a href="#">click here</a> <i class="fas fa-location-arrow"></i></h3>
        </div>

        <!-- testo italiano -->
        <div v-if="lingua=='italian'">
            <img src="../assets/DenixLogo.png" alt="Fox logo" class="logo">
            <p class="upper">Con la mia carriera da freelancer voglio offrire un <span class="highlit">servizio di qualità</span>, a un prezzo ragionevole siccome sto ancora imparando. Non inizierò la mia attività fino a quando non sarò abbastanza confidente <span class="highlit">di poter creare quasi qualsiasi cosa</span> un mio cliente possa chiedere. Durante la mia esperienza <span class="highlit">creerò dei pre-set</span> tra i quali i clienti possano scegliere, nel caso volessero un sito più economico. I preset sono meno personalizzabili, ma anche un punto di partenza per un sito completamente personalizzato. </p>
            <p class="lower">Tenete a mente che, anche se sono un full-stack developer, per adesso sono <span class="highlit">orientato al front-end</span>. Questo vuol dire che sto consolidando le mie skill da front-end più che quelle da back-end. Dunque se volete un sito con un database, mi ci vorrà <span class="highlit">più tempo</span> per completarlo, ma riuscirò comunque a farlo. In futuro completerò le mie conoscenze con anche abilità complete da back-end.</p>
            <h3>Se volete sapere di più sui miei piani, <a href="#">clicca qui</a> <i class="fas fa-location-arrow"></i></h3>
        </div>

        <!-- testo rumeno -->
        <div v-if="lingua=='romenian'">
            <img src="../assets/DenixLogo.png" alt="Fox logo" class="logo">
            <p class="upper">Cu cariera mea de freelancer vreau sa ofer un <span class="highlit">serviciu de calitate</span>, la un pret vantajos cum ca inca invat. Nu imi voi incepe activitatea pana nu sunt destul de confident <span class="highlit">cca pot sa fac aproape ori ce</span> un client imi va cere. Pe parcursul carierei voi <span class="highlit">crea niste pre-seturi</span> printe care clienti sa poata alege, in caz de vor un site mai economic. Pre-seturile vor fi mai putin personalizabile, dar pot fi si un punct de inceput pentru un site total personalizat.</p>
            <p class="lower">Tineti minte ca chear de sunt un full-stack developer, momentan sunt <span class="highlit">orientat la front-end</span> developer. Asta inseamna ca imi voi imbunatati abilitatile de front-end intai. Asa deci daca vreti un website cu database, imi va lua <span class="highlit">mai mult timp</span> sa il completez, dar tot voi reusi sa il fac. Pe viitor voi completa abilitatile mele cu skilluri de back-end.</p>
            <h3>Pentru a afla mai multe despre planul meu, <a href="#">apasati aici</a> <i class="fas fa-location-arrow"></i></h3>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Job',
    props: {
        lingua: String
    }
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';

    .job_desc {
        height: 60vh;
        padding-right: 20px;
        background-image: linear-gradient(black, $opposite_color);
        .upper {
            padding-top: 6%;
            margin-bottom: 3%;
            color: $main_color;
        }
        h3 {
            margin-top: 3%;
            color: $main_color;
            font-weight: 600;
            a {
                color: $main_color;
            }
        }
    }
    .logo {
        float: left;
        height: 50vh;
        margin-top: 10vh;
    }
    .fa-location-arrow {
        position: relative;
        z-index: 1;
        top: 20px;
        right: 10px;
        transform: rotate(270deg);
        animation: click_anim 4s infinite;
    }
</style>