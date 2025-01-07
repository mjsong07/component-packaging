<!-- 子组件 --> 
<template>
  <el-input :model-value="modelValue" @input="$emit('update:modelValue', $event)" >
    <!--(_, name)  注意第一个是内容，第二个才是key 也就是插槽的名称  -->
    <template v-for="(_, name) in $slots" #[name]="scopedData">
      <slot :name="name" v-bind="scopedData"></slot>
    </template>
  </el-input> 
</template>

<script>
export default {
  props: ['modelValue'],
  mounted() {
    console.log(this.$slots);
  }
}; 
</script>