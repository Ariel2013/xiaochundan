<template>
  <div>
    <div class="home_banner" id="home_banner">
      <canvas id='canvas' class="canvas"></canvas>
      <div class="nav_logo">纯指甲</div>
    </div>
    <!--<el-menu theme="dark" :default-active="activeIndex" class="el-menu-demo nav_menu" mode="horizontal" @select="handleSelect">-->
      <!--<el-menu-item>处理中心666</el-menu-item>-->
      <!--<el-menu-item index="1" class="nav">处理中心</el-menu-item>-->
      <!--<el-menu-item index="2" class="nav">订单管理</el-menu-item>-->
    <!--</el-menu>-->
    <!--<div>-->
      <!--666-->
    <!--</div>-->
    <!--<el-button @click="diyfun">按钮</el-button>-->
    <!--<div v-on:click="diyfun">click</div>-->
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
    width: 100%;
    height: auto;
    text-align: center;
  }
  .canvas {
    background: #000;
  }
  /*.home_bg:before {*/
    /*content: ''*/
    /*display: block !important*/
    /*position: absolute*/
    /*top: 0*/
    /*left: 0*/
    /*width: 100%*/
    /*height: 100%*/
    /*background: rgba(0,0,0,0.39)*/
    /*-webkit-transform: translate3d(0,0,0)*/
    /*transform: translate3d(0,0,0)*/
  /*}*/
  .nav_menu {
    display: inline-block
  }
  .home_banner {
    height: 600px;
  }
  .nav_logo {
    color: aliceblue;
    z-index: 100;
    position: absolute;
    top: 100px;
    left: 100px;
    font-size: x-large;
  }
</style>
<script>
  import myfun from '../assets/canvas.js'
  import util from '../assets/util.js'
  import '../assets/reset.css'
  export default {
    name: 'home',
    data () {
      return {}
    },
    mounted: function () {
      myfun()
    },
    methods: {
      diyfun: function () {
        myfun()
//        console.log(myfun)
        util()
      }
    }
  }

</script>
