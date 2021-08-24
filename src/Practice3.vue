<template>
  <p v-pre>{{age}}</p>
</template>
<script>
// import SlotsComponent from "./components/SlotsComponent.vue";
export default {
  name: "Practice3",
  components: {
    // SlotsComponent,
  },
  data(){
    return{
      age:10,
    }
  }
};
</script>

<style scoped>
p{
    font-size: 2rem;
    color: black;
}span{
    color:rgb(248, 181, 126);
}
</style>
