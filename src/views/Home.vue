<template>
  <div id="home">
    <!-- banner -->
    <Banner/>

    <!--专题-->
    <div class="subject-wrap">
      <Subject/>
    </div>
  </div>
</template>

<script>
import Banner from "@/components/Home/Banner";
import Subject from "@/components/Home/Subject";

export default {
  name: "Home",
  components: {
    Banner,
    Subject
  }
}
</script>

<style scoped>
#home {
  /*width: 1200px;*/
  margin: auto;
}

.subject-wrap {
  width: 1160px;
  margin: auto;
}
</style>