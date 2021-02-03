<template>
  <div id="banner">
    <el-carousel height="200px" type="card">
      <el-carousel-item
        v-for="bannerSrc in bannerSrcs"
        :key="bannerSrc"
        style="box-shadow: 2px 2px 2px #cccccc"
      >
        <img :src="bannerSrc" width="800px" height="300px">
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default {
  name: "Banner",
  data: () => {
    return {
      bannerSrcs: [
        require('@/assets/banner/banner1.jpg'),
        require('@/assets/banner/banner2.jpg'),
        require('@/assets/banner/banner3.jpg'),
        require('@/assets/banner/banner4.jpg')
      ]
    }
  }
}
</script>

<style scoped>
.el-carousel__item h3 {
  color: #475669;
  font-size: 14px;
  opacity: 0.75;
  line-height: 150px;
  margin: 0;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n+1) {
  background-color: #d3dce6;
}
</style>