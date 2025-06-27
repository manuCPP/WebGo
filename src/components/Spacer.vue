<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  space: String,
})


const space = props.space + 'rem'
</script>


<template>
  <div ></div>
</template>

<style scoped>
  div{
    height: v-bind(space);
    width: 100vw;
    

  }
</style>
