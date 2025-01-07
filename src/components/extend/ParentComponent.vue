<template>
   <ChildComponent id="child" class="custom-class" data-custom="123"   />  
  </template>
  
  <script>
  import ChildComponent from './ChildComponent.vue'; 
  
  export default {
    components: {
        ChildComponent, 
    },
    data() { 
    
    }
  };
  </script> 