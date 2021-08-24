<template>
  <div class="container p-2">
    <!-- 1 -->
    <ul>
      <li v-for="lang in listOne" :key="lang">
{{lang}}
      </li>
    </ul>
    <!-- 2 -->
   <p v-if="listTwo.length>0">list length is {{listTwo.length}}</p>
  </div>
</template>

<script>
export default {
  name: "Practice1",
  components: {},

  data() {
    return {
      listOne: ["HTML", "Css", "JavaScript", "Vue.js", "React.js"],
      listTwo: ['0'],
    };
  },
};
</script>

<style scoped>
</style>
