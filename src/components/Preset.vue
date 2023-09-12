<template>
    <div class="preSetContainer">
        <div class="card">
            <h2 class="title">Renata's Website</h2>
            <div>
                <a href="https://flamboyant-spence-68b208.netlify.app/">
                    <img src="../assets/Screenshot 2023-09-12 210128.png" alt="Renata screenshot">
                </a>
            </div>
            <p>Pre set short description of about 50 words</p>
            <p>Preset popularity from 1 to 5 stars</p>
        </div>
        <!-- <div class="card">
            <h2 class="title">PreSet name</h2>
            <img src="" alt="PreSet screen">
            <p>Pre set short description of about 50 words</p>
            <p>Preset popularity from 1 to 5 stars</p>
        </div>
        <div class="card">
            <h2 class="title">PreSet name</h2>
            <img src="" alt="PreSet screen">
            <p>Pre set short description of about 50 words</p>
            <p>Preset popularity from 1 to 5 stars</p>
        </div>
        <div class="card">
            <h2 class="title">PreSet name</h2>
            <img src="" alt="PreSet screen">
            <p>Pre set short description of about 50 words</p>
            <p>Preset popularity from 1 to 5 stars</p>
        </div> -->
    </div>
</template>

<script>
export default {
    name: 'Preset',
    props: {
        lingua: String
    }
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';

.preSetContainer {
    display: flex;
    justify-content: space-around;
    padding: 30px;
    background-image: linear-gradient($opposite_color, black);
}

.card {
    display: inline-block;
    width: 200px;
    height: 300px;
    padding: 5px;
    border: 2px solid black;
    background-image: linear-gradient(black, $opposite_color);
    color: white;

    a {
        img {
            width: 100%;
        }
    }

}
</style>