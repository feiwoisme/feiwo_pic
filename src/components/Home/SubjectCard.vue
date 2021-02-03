<template>
  <div id="subject_card">
    <el-card :body-style="{ padding: '0px' }">
      <div class="title-wrap">
        <div class="title">{{ subject.title }}</div>
      </div>
      <div class="cover-wrap">
        <div style="overflow: hidden">
          <img :src="subject.cover" width="100%" height="180px">
        </div>
      </div>
      <div class="intro-wrap">
        {{ subject.intro }}
      </div>
    </el-card>
  </div>
</template>

<script>
export default {
  name: "SubjectCard",
  props: {
    subject: {
      id: Number,
      title: String,
      cover: String,
      intro: String
    }
  }
}
</script>

<style scoped>
#subject_card {
  cursor: pointer;
}

.title-wrap {
  padding: 10px 10px;
  border-bottom: 1px solid #EBEEF5;
  box-sizing: border-box;
}

.title {
  padding: 5px;
  padding-left: 8px;  border-left: 6px solid #99a9bf;
  font-weight: 600;
  color: #555555;
}

.cover-wrap {
  padding: 10px;
}

.cover-wrap img {
  transition: all .5s;
}

.cover-wrap:hover img {
  transform: scale(1.1);
}

.intro-wrap {
  margin: 15px;
  margin-top: 0;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}
</style>