<template>
  <div class="home_bg">
    <div>
      666
    </div>
  </div>
</template>
<style>
  .home_bg {
    background-repeat: no-repeat;
    background-size: cover;
    background-color: transparent;
    background-position: 50% 50%;
    background-image: url('../assets/home_bg.jpg');
    background-attachment: fixed;
  }
  .home_bg:before {
    content: '';
    display: block !important;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.39);
    -webkit-transform: translate3d(0,0,0);
    transform: translate3d(0,0,0);
  }
</style>
<script>
  export default {
    name: 'home',
    data () {
      return {}
    }
  }
</script>
