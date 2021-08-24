<template>
<!-- 
<p>  name</p>
<p v-text="name"></p>
<p v-html="name"></p>
<ul>
  <li v-for="(list,index) in lists" :key="index">{{list + index}}</li>
</ul>

<p v-if="age==10">you are 10</p>
<p v-else-if="age>10">you bigger than 10</p>
<p v-else>you are small</p>
<img v-bind:src="imgSrc" alt=""> -->
<!-- <button @click="sayhi">Click</button> -->


<!-- <p v-once>{{counter}}</p>
<button @click="counter++">Click</button>
<p v-pre>{{age}}</p> -->
<!-- p1 -->
<!-- <practice1/> -->

<!-- p2 -->
<!-- <practice2/> -->

<!-- p2 -->
<!-- <practice3/> -->

  <h1 class="w-50 m-auto p-4 text-center">Sign up</h1>
  <FormCard />
<!-- <p v-show="show">Show Element</p>
<p v-if="show">Show Element</p> -->
  <div class="circle"></div>
</template>

<script>
// import Practice1 from './Practice1.vue';
// import Practice2 from './Practice2.vue';
// import Practice3 from './Practice3.vue';
import FormCard from "./components/FormCard.vue";
import imgSrc from './assets/logo.png';
export default {
  name: "App",
  components: {
    // Practice1,
    // Practice3,
    // Practice2,
    FormCard,
  },
  data(){
    return{
      lists:['1','2','3','4'], //loop
      longSentance:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate labore quod illo laudantium aliquid, quibusdam officia perferendis ea eos, similique vero sint, quasi exercitationem fugit dicta et blanditiis! Ipsam, suscipit?',
      name:'<p>Nada</p>',
      imgSrc:imgSrc,
      age:5,
      classOne:'col-6',
      show:true,
      counter:1,
    }
  },
  methods:{
    sayhi(){
      alert('hi')
    },
    toggleShow(){
      this.show = !this.show
    },
  }
};
</script>

<style>
body {
  background: white;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  height: 100vh;
  overflow: hidden;
}

.circle {
  width: 500px;
  height: 500px;
  border-radius: 50%;
  background-color: #fff2ee;
  position: absolute;
  bottom: -20%;
  left: -10%;
  z-index: -1;
}
</style>
