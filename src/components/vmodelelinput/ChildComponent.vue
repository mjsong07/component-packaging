<!-- 子组件 --> 
<template>
  <el-input :model-value="modelValue" @input="$emit('update:modelValue', $event)" > 
   </el-input> 
</template>

<script>
export default {
  props: ['modelValue'],
};
</script>