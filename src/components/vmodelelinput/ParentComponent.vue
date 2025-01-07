<template>
   <MidComponent v-model="parentData" />  
  </template>
  
  <script>
  import MidComponent from './MidComponent.vue'; 
  
  export default {
    components: {
        MidComponent,  
    },
    data() {
        return {
            parentData:  'xxxx'
        };
        }
  };
  </script> 