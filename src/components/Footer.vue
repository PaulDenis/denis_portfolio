<template>
    <div class="footer_container">
        <div class="left_footer">

        <!-- Footer inglese -->
            <ul class="footer_menu"
            v-if="lingua=='american english'">
                <li><a href="#">Home</a></li>
                <li><a href="#">About me</a></li>
                <li><a href="#">Projects</a></li>
                <li><a href="#">Gallery</a></li>
                <!-- <li><a href="#">Pre-Sets</a></li> -->
            </ul>

            <!-- Footer italiano -->
            <ul class="footer_menu"
            v-if="lingua=='italian'">
                <li><a href="#">Home</a></li>
                <li><a href="#">Su di me</a></li>
                <li><a href="#">Progetti</a></li>
                <li><a href="#">Galleria</a></li>
                <!-- <li><a href="#">Pre-sets</a></li> -->
            </ul>

            <!-- Footer rumeno -->
            <ul class="footer_menu"
            v-if="lingua=='romanian'">
                <li><a href="#">Home</a></li>
                <li><a href="#">Despre mine</a></li>
                <li><a href="#">Proiecte</a></li>
                <li><a href="#">Galerie</a></li>
                <!-- <li><a href="#">Pre-sets</a></li> -->
            </ul>
            <ul class="inline_menu">
                <li><a href="#"><i class="fab fa-instagram"></i></a></li>
                <li><a href="#"><i class="fab fa-youtube"></i></a></li>
                <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
                <li><a href="#"><i class="fab fa-tiktok"></i></a></li>
                <li><a href="#"><i class="fab fa-linkedin"></i></a></li>
            </ul>
        </div>
        <p v-if="lingua=='american english'">&copy; copyright preotected</p>
        <p v-if="lingua=='italian'">&copy; Protetto da copyright</p>
        <p v-if="lingua=='romanian'">&copy; protejat de copyright</p>

        <div class="right_footer">
            <ul>
                <li v-if="lingua=='american english'">Contact me</li>
                <li v-if="lingua=='italian'">Contattami</li>
                <li v-if="lingua=='romanian'">Contacteaza-ma</li>
                <li><a href="#">+39 123 123 1234</a></li>
                <li><a href="#">d.paul@outlook.it</a></li>
                <li><a href="#">Via roma 1 - Modena, Italy</a></li>

            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Footer',
    props: {
        lingua: String
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/common.scss';

.footer_container {
    display: flex;
    justify-content: space-between;
    padding-top: 20px;
    border-top: 3px solid black;
    background-color: $opposite_color;
    p {
        margin-top: 150px;
        font-size: 10px;
    }
}
ul {
    list-style: none;
    padding: 0;
    margin: 0;
    padding-left: 20px;
    padding-bottom: 20px;
    li {
        a {
            text-decoration: none;
            color: black;
        }
    }
}
.inline_menu {
    li {
        display: inline-block;
        margin-top: 0;
        margin: 10px;
        &:first-child {
            margin-left: 0;
        }

    }
}
.right_footer {
    ul {
        margin-right: 20px;
        li {
            text-align: right;
            &:first-child {
                font-size: 20px;
                font-weight: 600;
            }
        }
    }
}
</style>