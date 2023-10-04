<template>
  <example-model/>
</template>

<script lang="ts">

import { defineComponent } from 'vue';
import ExampleSelective from './components/ExampleSelective.vue';
import ExampleFor from './components/ExampleFor.vue';
import ClassBind from './components/ClassBind.vue';
import ExampleModel from './components/ExampleModel.vue';

export default defineComponent({
  components :{
    ExampleSelective,
    ExampleFor,
    ClassBind,
    ExampleModel
  }
})

</script>

<style lang="scss" scoped>

</style>
