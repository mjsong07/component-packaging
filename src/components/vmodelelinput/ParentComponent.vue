<template>

  <h1>vmodelelinput</h1>
   <MidComponent v-model="parentData" :parentData2="parentData2" />  
   <input type="button" value="test" @click="test">
  </template>
  
  <script>
  import MidComponent from './MidComponent.vue'; 
  
  export default {
    components: {
        MidComponent,  
    },
    data() {
        return {
            parentData:  'xxxx',
            parentData2:  'xxxx'
        };
        },   methods: {
        test() { 
            this.parentData2 = "dddd"
            console.log("parentData",this.parentData)
            console.log("parentData2",this.parentData2)
        }
    }
  };
  </script> 