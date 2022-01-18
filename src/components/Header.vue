!<template>
  <div class="container">
      <img src="../assets/DenisPicture.jpg" alt="">
      <div class="fading">
          <h1>Hi, my name is Denis and i'm from italy</h1>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss" scoped>
    .container {
        width:100%;
        height: 100%;
        position:relative;
    }
    .fading{
        position: absolute;
        top: 0;
        left: 50%;
        transform: translateX(-50%);
        width:50%;
        height:100vh;
        text-align: left;
        padding-left: 120px;

        background: rgba(255,255,255,0.9);
        background: -moz-linear-gradient(left, rgba(255,255,255,1) 0%, rgba(255,255,255,0.9) 15%, rgba(255,255,255,0) 50%, rgba(255,255,255,0.9) 85%, rgba(255,255,255,0.9) 100%);
        background: -webkit-gradient(left top, right top, color-stop(0%, rgba(255,255,255,0.9)), color-stop(15%, rgba(255,255,255,0.9)), color-stop(50%, rgba(255,255,255,0)), color-stop(85%, rgba(255,255,255,0.9)), color-stop(100%, rgba(255,255,255,0.9)));
        background: -webkit-linear-gradient(left, rgba(255,255,255,0.9) 0%, rgba(255,255,255,0.9) 15%, rgba(255,255,255,0) 50%, rgba(255,255,255,0.9) 85%, rgba(255,255,255,0.9) 100%);
        background: -o-linear-gradient(left, rgba(255,255,255,0.9) 0%, rgba(255,255,255,0.9) 15%, rgba(255,255,255,0) 50%, rgba(255,255,255,0.9) 85%, rgba(255,255,255,0.9) 100%);
        background: -ms-linear-gradient(left, rgba(255,255,255,0.9) 0%, rgba(255,255,255,0.9) 15%, rgba(255,255,255,0) 50%, rgba(255,255,255,0.9) 85%, rgba(255,255,255,0.9) 100%);
        background: linear-gradient(to right, rgba(255,255,255,1) 0%, rgba(255,255,255,0.7) 45%, rgba(255,255,255,0) 70%);
        filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#ffffff', endColorstr='#ffffff', GradientType=1 );
    }


</style>