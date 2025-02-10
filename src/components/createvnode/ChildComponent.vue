 

<script lang="ts">
import { computed, createVNode, defineComponent, resolveComponent } from 'vue' 
import ChildSubComponent from './ChildSubComponent.vue'; 
export default defineComponent({ 
  props: { 
    modelValue: {
      required: true,
    }, 
  },
  emits: ['update:modelValue'], 
  setup(props, { emit }) {
    const onValueUpdate = (value: any) => {
      emit('update:modelValue', value)
    } 

      return () =>
       createVNode(ChildSubComponent, { 
        modelValue: props.modelValue, 
        'onUpdate:modelValue': onValueUpdate, 
      })
  },
})
</script>
 