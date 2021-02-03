<template>
  <div id="footer">
    <div>
      <img :src="weixin" width="18" class="icon">
      <span class="text">j1005098087</span>
      <el-tooltip placement="top" effect="light">
        <div slot="content">
          <img :src="erweima" width="120px">
        </div>
        <img :src="QRcode" width="18" class="QRcode">
      </el-tooltip>
    </div>
    <span class="line">|</span>
    <div>
      <img :src="QQ" width="18" class="icon">
      <span class="text">1005098087</span>
      <el-tooltip placement="top" effect="light">
        <div slot="content">
          <img :src="erweima" width="120px">
        </div>
        <img :src="QRcode" width="18" class="QRcode">
      </el-tooltip>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data: () => {
    return {
      weixin: require('@/assets/icon/weixin.png'),
      QQ: require('@/assets/icon/QQ.png'),
      QRcode: require('@/assets/icon/QR-code.png'),
      erweima: require('@/assets/erweima.png')
    }
  }
}
</script>

<style scoped>
#footer {
  display: flex;
  justify-content: center;
  position: relative;
  padding: 60px;
  text-align: center;
}

.icon {
  position: relative;
  top: 4px;
}

.text {
  margin-left: 5px;
}

.line {
  margin: 0 40px;
  line-height: 1.5rem;
  color: #ccc;
}
.QRcode {
  position: relative;
  top: 4px;
  margin-left: 5px;
}
</style>