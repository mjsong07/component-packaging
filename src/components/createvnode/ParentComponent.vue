<template>
    <h1>createvnode</h1>
    <MidComponent v-model="parentData"  />  
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
         };
         },   methods: {
         test() {  
             console.log("xxxx",this.parentData)
         }
     }
   };
   </script> 