<template>

  <h1>vmodel</h1>
   <MidComponent v-model="parentData" /> 
   <!-- <MidComponent :modelValue="parentData" @update:modelValue="parentData = $event" />  -->
  </template>
  
  <script>
  import MidComponent from './MidComponent.vue';
  import ChildComponent from './ChildComponent.vue';
  
  export default {
    components: {
        MidComponent,
        ChildComponent,
    },
    data() {
        return {
            parentData:  'xxxx'
        };
        }
  };
  </script> 