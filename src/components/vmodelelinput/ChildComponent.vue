<!-- 子组件 --> 
<template>
  <div> 
   <el-input :model-value="modelValue" @input="$emit('update:modelValue', $event)" > 
  </el-input>  

  <el-input :model-value="parentData2"   > 
  </el-input>  
  </div>
 
</template>

<script>
export default {
  props: ['modelValue','parentData2'], 
};
</script>