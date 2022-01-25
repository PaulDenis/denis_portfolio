<template>
    <div class="footer_container">
        <div class="left_footer">
            <ul class="footer_menu">
                <li><a href="#">Home</a></li>
                <li><a href="#">About me</a></li>
                <li><a href="#">Projects</a></li>
                <li><a href="#">Gallery</a></li>
                <!-- <li><a href="#">Pre-Sets</a></li> -->
            </ul>
            <ul class="inline_menu">
                <li><a href="#"><i class="fab fa-instagram"></i></a></li>
                <li><a href="#"><i class="fab fa-youtube"></i></a></li>
                <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
                <li><a href="#"><i class="fab fa-tiktok"></i></a></li>
                <li><a href="#"><i class="fab fa-linkedin"></i></a></li>
            </ul>
        </div>
        <p>&copy; copyright preotected</p>
        <div class="right_footer">
            <ul>
                <li>Contact me</li>
                <li><a href="#">+39 123 123 1234</a></li>
                <li><a href="#">d.paul@outlook.it</a></li>
                <li><a href="#">Via roma 1 - Modena, Italy</a></li>

            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Footer'
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