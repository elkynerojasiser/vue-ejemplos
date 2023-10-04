<template>
<h1 v-show="visible">Soy un elemento</h1>

</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    data() {
        return {
            visible: false,
            age:70
        }
    }
})

</script>

<style lang="scss" scoped>
</style>