<template>
    <div class="footer_container">
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
        </ul>
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
    border-top: 3px solid black;
    background-color: $opposite_color;
}
.footer_menu {
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
    list-style: none;
    padding: 0;
    margin: 0;
    padding-left: 20px;
    padding-bottom: 20px;
    li {
        display: inline-block;
        margin-top: 0;
        margin: 10px;
            &:first-child {
            margin-left: 0;
        }
        a {
            text-decoration: none;
            color: black;
        }
    }
}

</style>