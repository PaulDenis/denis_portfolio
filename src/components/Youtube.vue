<template>
  <div class="YoutubeContainer">
    <iframe width="420" height="315"
    src="https://www.youtube.com/embed/OtUy_Dbqjhs" class="YTvideo">
    </iframe>

    <!-- testo YT inglese -->
    <div v-if="lingua=='american english'">
        <h2>Latest Youtube Video</h2>
        <p>As I already told, I own a YouTube channel. It's all about programming. I give tips, trick and do tutorials of all kind.</p>
        <p>If you want to know more about me, my skills and my personality, YouTube is the best way to quickly make an idea about all that.</p>
        <p>The one on the left is the latest video that I uploaded, but you can find a lot more by clicking <a href="https://www.youtube.com/channel/UCFPJIxOlhBsz9AvV8iYDu9Q" target="_blank">Here</a></p>
    </div>

    <!-- testo YT italiano -->
    <div v-if="lingua=='italian'">
        <h2>Ultimo video su YouTube</h2>
        <p>Come vi ho già detto, ho un canale YouTube. E' basato completamente sulla programmazione. Do consigli, trucchi e faccio tutorial di ogni tipo.</p>
        <p>Se volete sapere di più su di me, le mie abilità e la mia personalità, YouTube è la scelta migliore per farvi una rapida idea su tutto.</p>
        <p>Quello sulla sinistra è l'ultimo video che ho pubblicato, ma potete trovarne di più <a href="https://www.youtube.com/channel/UCFPJIxOlhBsz9AvV8iYDu9Q" target="_blank">cliccando qui</a></p>
    </div>

    <!-- testo YT rumeno -->
    <div v-if="lingua=='romanian'">
        <h2>Ultimu video pe YouTube</h2>
        <p>Cum v-am zis deja, detin un canal YouTube. Se bazeaza pe programare. Dau sfaturi, 'trucuri' si multe feluri de tutoriale.</p>
        <p>Daca vreti sa stiti mai multe despre mine, personalitatea si abilitatile mele, YouTube ii cea mai buna cale sa va faceti o idee rapida despre toate.</p>
        <p>Cel pe stanga este ultimul video incarcat, dar puteti gasi mai multe <a href="https://www.youtube.com/channel/UCFPJIxOlhBsz9AvV8iYDu9Q" target="_blank">apasand aici</a></p>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Youtube',
    props: {
        lingua: String
    }
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