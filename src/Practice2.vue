<template>
  <div class="container p-2">
    <p :class="className">Class Binding</p>
    <button class="btn btn-primary" @click="toggleClass">
      Toggle Class Name
    </button>
    <input class="d-block my-2" type="text" v-model="inputValue">
    <p>{{inputValue}}</p>
  </div>
</template>

<script>
export default {
  name: "Practice2",
  methods: {
    toggleClass() {
      if (this.className == "red") {
        this.className = "blue";
      } else {
        this.className = "red";
      }
    },
  },
  data() {
    return {
      className: "red",
      inputValue:''
    };
  },
};
</script>

<style scoped>
.red {
  color: red;
}
.blue {
  color: blue;
}
</style>
