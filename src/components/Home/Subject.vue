<template>
  <div id="subject">
    <el-row :gutter="30">
      <el-col
        :span="6"
        v-for="subject in subjects"
        :key="subject.id"
        style="margin-top: 2rem;"
      >
        <SubjectCard :subject="subject"/>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import SubjectCard from "@/components/Home/SubjectCard";

export default {
  name: "Subject",
  data: () => {
    return {
      subjects: [
        {
          id: 1,
          title: '鸟语花香',
          cover: require('@/assets/cover/cover1.jpg'),
          intro: '清晨，打开窗户，让春风透过纱窗絮絮地吹进屋里，聆听着窗外鸟儿欢快的叫声，合上双眼，一副鸟语花香、万物复苏的场景呈现在眼前。'
        },
        {
          id: 2,
          title: '晨风露雨',
          cover: require('@/assets/cover/cover2.jpg'),
          intro: '清晨呼吸着山里新鲜的空气，聆听者窗外鸟儿的鸣叫，看着那满山遍野盛开的油菜花。'
        },
        {
          id: 3,
          title: '随想',
          cover: require('@/assets/cover/cover3.jpg'),
          intro: '此心安处是吾乡。'
        },
        {
          id: 4,
          title: '阅读',
          cover: require('@/assets/cover/cover4.jpg'),
          intro: '吹灭读书灯，一身皆是月。'
        },
        {
          id: 5,
          title: '自由',
          cover: require('@/assets/cover/cover5.jpg'),
          intro: '吹灭读书灯，一身皆是月。'
        },
        {
          id: 6,
          title: '飞翔',
          cover: require('@/assets/cover/cover6.jpg'),
          intro: '吹灭读书灯，一身皆是月。'
        },
        {
          id: 7,
          title: '阅读',
          cover: require('@/assets/cover/cover7.jpg'),
          intro: '吹灭读书灯，一身皆是月。'
        },
        {
          id: 8,
          title: '图书馆',
          cover: require('@/assets/cover/cover8.jpg'),
          intro: '吹灭读书灯，一身皆是月。'
        },
        {
          id: 9,
          title: '梦',
          cover: require('@/assets/cover/cover9.jpg'),
          intro: '吹灭读书灯，一身皆是月。'
        },
        {
          id: 10,
          title: '事业',
          cover: require('@/assets/cover/cover10.jpg'),
          intro: '吹灭读书灯，一身皆是月。'
        },
        {
          id: 11,
          title: '徒行',
          cover: require('@/assets/cover/cover11.jpg'),
          intro: '吹灭读书灯，一身皆是月。'
        },
        {
          id: 12,
          title: '成长',
          cover: require('@/assets/cover/cover12.jpg'),
          intro: '吹灭读书灯，一身皆是月。'
        }
      ]
    }
  },
  components: {
    SubjectCard
  }
}
</script>

<style scoped>
</style>