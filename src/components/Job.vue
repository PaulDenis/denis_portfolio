<template>
    <div class="job_desc">
        <img src="../assets/DenixLogo.png" alt="Fox logo" class="logo">
        <p class="upper">With my Freelancing career I want to offer <span class="highlit">good quality service</span>, at a fair price since I am still learning. I won't start my activity until I am not confident enough that <span class="highlit">I can create almost anything</span> my client will ask for. During my experience I will <span class="highlit">create some pre-sets</span> for the clients to choose from, in case they want a cheaper website. The presets will be less personalizable, but also a starting point for a completly personalized website. </p>
        <p class="lower">Keep in mind that, even if I' am a full stack, for now I am a <span class="highlit">front-end oriented</span> developer. That means that for now I am improving my front-end skills more than the back-end skills. So if you want a website with a database, it will take <span class="highlit">more time</span> for me to complete it, but I can still do it. In the future I will complete my knowlege with back-end services too.</p>
        <h3>To read more about my plan, <a href="#">click here</a> <i class="fas fa-location-arrow"></i></h3>
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