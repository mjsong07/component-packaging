<template>

  <h1>ref</h1>
   <ChildComponent ref="testRef" v-model="parentData" />  
   <input type="button" value="test" @click="test">
  </template>
  
  <script>
  import ChildComponent from './ChildComponent.vue'; 
  
  export default {
    components: {
        ChildComponent,  
    },
    data() {
        return {
            parentData:  'xxxx'
        };
    },
    methods: {
        test() {
            this.$refs.testRef.focus2()
            console.log(this.$refs.testRef.val)
        }
    }
  };
  </script> 