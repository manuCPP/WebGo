<script setup>
import { defineProps } from 'vue'
import { computed } from 'vue'

const props = defineProps({
  size: String,
  img: String

});


function resolveImagePath(path) {
  return new URL(`../assets/images/${path}`, import.meta.url).href;
}
console.log(props.img)
const imgSrc = resolveImagePath(props.img)


const size = props.size + 'rem';
</script>

<template>
  <div><img width="50%" :src="imgSrc" alt="immagine impossibile da caricare"/></div>
</template>


<style scoped>


div{
  border-radius: 50%;
  background-color: var(--primary-color);
  width: v-bind(size);
  height: v-bind(size);

  display: flex;
  align-items: center;
  justify-content: center;
}

</style>
