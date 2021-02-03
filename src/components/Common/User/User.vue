<template>
  <div id="user">
    <div class="bg">
      <div class="half-circle"></div>
      <div class="rect"></div>
    </div>
    <div class="avatar-wrap">
      <img :src="avatarSrc" class="avatar" height="35px">
      <img :src="menuSrc" height="12px">
      <!--            肥我-->
    </div>
  </div>
</template>

<script>
export default {
  name: "User",
  data: () => {
    return {
      menuSrc: require('@/assets/icon/menu.png'),
      avatarSrc: require('@/assets/avatar.jpg')
    }
  }
}
</script>

<style scoped>
#user {
  display: flex;
}
.avatar-wrap {
  display:flex;
  align-items:center;
  margin-left: -107px;
}

.bg {
  display: flex;
}
.rect {
  padding: 3px 10px;
  background: #dddddd;
  width: 40px;
}
.half-circle {
  margin-left: -20px;
  border: 20px solid #dddddd;
  border-radius: 50% 0 0 50%;
}

.avatar {
  margin: 0 10px;
  border-radius: 50%;
}
</style>