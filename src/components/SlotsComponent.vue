<template>
<div class=" p-5">
  <slot name="slotOne"></slot> 
  </div>
  
  <slot name="slotTwo"></slot> 

  -------------
  <slot name='slotThree'></slot>
</template>
<script>
export default {
  name: "SlotsComponent",
};
</script>
<style scoped>
*{
    color: white;
    font-weight: bold;
    text-align: center;
}
</style>