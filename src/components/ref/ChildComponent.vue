<!-- 子组件 --> 
<template>
  <el-input ref="myRef" :model-value="modelValue" @input="$emit('update:modelValue', $event)" > 
   </el-input> 
</template>

<script>
export default {
  props: ['modelValue'],
  data() {
    return {
      val:111
    } 
  },
  mounted() { 
    for (const key in this.$refs.myRef) {
        this[key] = this.$refs.myRef[key]
    } 
  },
  methods: {
    focus2() {
      this.$refs.myRef.focus()
    }
  }

};
</script>