<template>
    <div class="job_desc">
        <img src="../assets/DenixLogo.png" alt="Fox logo" class="logo">
        <p class="upper">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sequi modi nihil dolorum nisi porro explicabo eveniet accusamus reiciendis iste eos quod commodi magni, voluptatem qui officiis? Soluta ut facere, nesciunt quidem sunt minus voluptate delectus debitis tenetur sed id aspernatur, laborum ea. Maiores deleniti quam libero, sint animi nulla temporibus sapiente sequi aperiam, beatae autem maxime quisquam. Velit vel dicta rerum eligendi consequuntur quo error nulla, sapiente, asperiores laudantium enim? </p>
        <p class="lower">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sequi modi nihil dolorum nisi porro explicabo eveniet accusamus reiciendis iste eos quod commodi magni, voluptatem qui officiis? Soluta ut facere, nesciunt quidem sunt minus voluptate delectus debitis tenetur sed id aspernatur, laborum ea. Maiores deleniti quam libero, sint animi nulla temporibus sapiente sequi aperiam, beatae autem maxime quisquam. Velit vel dicta rerum eligendi consequuntur quo error nulla, sapiente, asperiores laudantium enim? </p>
    </div>
</template>

<script>
export default {
    name: 'Job'
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';

    .job_desc {
        height: 60vh;
        background-image: linear-gradient(black, $opposite_color);
        .upper {
            padding-top: 5%;
            margin-bottom: 3%;
            color: $main_color;
        }
    }
    .logo {
        float: left;
        height: 50vh;
        margin-top: 10vh;
    }
</style>