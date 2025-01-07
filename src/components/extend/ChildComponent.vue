<template>
  <div v-bind="$attrs" id="child2"  >
    <!-- 子组件内容 -->
  </div>
</template>

<script>
export default {
  inheritAttrs: false, // 禁用根节点默认的属性继承
};
</script>