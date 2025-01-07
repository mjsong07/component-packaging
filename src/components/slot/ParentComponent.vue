<template>
    <MidComponent v-model="parentData"> 
        <template #prefix>
            111
        </template>
        <template #suffix>
            222
        </template> 
        <template #prepend>
            333
        </template>
    </MidComponent>
</template>

<script>
import MidComponent from './MidComponent.vue'; 
export default {
    components: {
        MidComponent, 
    },
    data() {
        return {
            parentData: 'xxxx'
        };
    }
};
</script>