<template>
  <h4 >welcome {{name}}</h4>
  <form @submit.prevent="sayhi">
    <div class="my-4">
      <span>user name :</span><input type="text" v-model="userNameVal"/>
      <p>{{userNameVal}}</p>
    </div>
    <div class="my-4"><span>password :</span><input type="password" /></div>
    <button type="submit" class="btn btn-secondary" >Submit</button>
  </form>
 
</template>


<script>
export default {
  name: "FormComponent",

props:{
  name:String,
},
data(){
  return{
    userNameVal:'nada'
  }
},
methods:{
  sayhi(){
    alert('hi')
  }
}
};
</script>


<style scoped>
h4 {
  font-weight: bold;
  text-transform: capitalize;
}
input,button{
    width: 250px;
    display: block;
}
button{
    background-color: #eee;
    color: black;
}
</style>