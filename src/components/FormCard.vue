<template>
  <div class="card w-75 m-auto">
    <div class="row">
      <div class="form-container col-6 p-5">
        <FormComponent name="Vue.js" />
        <!--  to bind props use v-bind:propname -->
      </div>
      <div class="slots-container col-6">
        <!-- <SlotsComponent> -->
        <!-- <template v-slot:slotOne>
            <p>kdkdkdkd</p>
          </template> -->
        <!-- </SlotsComponent> -->
        <SlotsComponent>
          <template v-slot:slotOne>
            <p>Slot</p>
          </template>
          <template v-slot:slotTwo>
            <p>Slot</p>
          </template>
        </SlotsComponent>
      </div>
    </div>
  </div>
</template>

<script>
import SlotsComponent from "./SlotsComponent.vue";
import FormComponent from "./FormComponent.vue";
export default {
  name: "FormCard",
  components: {
    SlotsComponent,
    FormComponent,
  },
  props: {
    msg: String,
  },
  data() {
    return {
      appName: "Vue.js",
    };
  },
};
</script>
<style scoped>
.card {
  overflow: hidden;
  box-shadow: 0 0 10px #ffc4b1;
  border-radius: 20px;
}
.slots-container {
  background-image: linear-gradient(rgb(253 207 125), rgb(252 63 134));
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
