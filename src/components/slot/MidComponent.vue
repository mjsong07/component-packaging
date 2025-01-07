<!-- 中间组件 -->
<template>
  <ChildComponent v-bind="$attrs"  >
    <template v-for="(_, name) in $slots" #[name]="scopedData">
    <slot :name="name" v-bind="scopedData"></slot>
    </template>
  </ChildComponent>

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