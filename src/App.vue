<template>
  <div id="app">
    <div class="user-wrap">
      <User></User>
    </div>

    <router-view/>

    <!--Footer-->
    <Footer/>

    <!--至顶部-->
    <el-backtop></el-backtop>

    <Background></Background>
  </div>
</template>

<script>
import Home from "@/views/Home";
import Footer from "@/components/Common/Footer";
import Background from '@/components/Common/Background';
import User from '@/components/Common/User/User';

export default {
  name: 'App',
  comments: {
    Home
  },
  components: {
    Footer,
    Background,
    User
  }
}
</script>

<style>
body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background: #f6f6f6;
  color: #2c3e50;
  font-size: 1rem;
}

.user-wrap {
  position: fixed;
  right: 10px;
  /*top: 20px;*/
  /*left: 0;*/
  /*z-index: 10;*/
  z-index: 10;
}
</style>
