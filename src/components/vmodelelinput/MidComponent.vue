<!-- 中间组件 -->
<template>
  <ChildComponent v-bind="$attrs"  />
</template>

<script>
import ChildComponent from './ChildComponent.vue';
export default {
  components: {
    ChildComponent,
  },
  inheritAttrs: false,
};
</script>