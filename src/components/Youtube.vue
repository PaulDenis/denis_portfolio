<template>
  <div class="YoutubeContainer">
    <iframe width="420" height="315"
    src="https://www.youtube.com/embed/OtUy_Dbqjhs" class="YTvideo">
    </iframe>
    <h2>Latest Youtube Video</h2>
    <p>As I already told, I own a YouTube channel. It's all about programming. I give tips, trick and do tutorials of all kind.</p>
    <p>If you want to know more about me, my skills and my personality, YouTube is the best way to quickly make an idea about all that.</p>
    <p>The one on the left is the latest video that I uploaded, but you can find a lot more by clicking <a href="https://www.youtube.com/channel/UCFPJIxOlhBsz9AvV8iYDu9Q" target="_blank">Here</a></p>
  </div>
</template>

<script>
export default {
    name: 'Youtube'
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';

.YoutubeContainer {
    background-color: $opposite_color;
    padding-bottom: 20px;
    padding-top: 50px;
    &::after {
        content:"";
        display: table;
        clear: both;
    }
    h2 {
        margin-bottom: 20px;
        font-weight: 600;
    }
    .YTvideo {
        margin-left: 50px;
        margin-right: 50px;
        float: left;
        border: 4px solid $main_color;
    }
}

</style>