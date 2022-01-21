<template>
    <!-- Una normale barra di navigazione, non troppo complessa in quanto si baserà principalmente sulla home -->
    <div>
        <ul class="inline_menu">
            <li><a href="#">Home</a></li>
            <li><a href="#">Projects</a></li>
            <li><a href="#">About me</a></li>
            <li><a href="#">Gallery</a></li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'NavBar'
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';

.inline_menu {
    list-style: none;
    display: inline-block;
    width: 100%;
    height: 35px;
    display: flex;
    align-items: center;
    position: fixed;
    top: 0;
    padding: 0;
    background-color: $opposite_color;
    // background-image: linear-gradient(to right, $opposite_color, white);
    li {
        padding-right: 30px;
        padding-left: 30px;
        border-right: 1px solid black;
        &:last-child {
            border: none;
        }
        a {
            color: black;
            text-decoration: none;
            font-weight: 700;
            &:hover {
                text-decoration: underline;
            }
        }
    }
}

</style>