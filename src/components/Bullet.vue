<script setup>
  import Circle from '@/components/Circle.vue';
  import { defineProps } from 'vue'

  const props = defineProps({
    title: String,
    body: String,
    img: String
  })

</script>

<template>
  <div class="bullet">
    <div class="headline">
        <Circle size="3" :img="props.img"/>
        <h2 style="text-wrap: nowrap;">{{ props.title }}</h2>
    </div>
    <div class="text">
        <p>{{ props.body }}</p>
    </div>
  </div>
</template>


<style scoped>
  .headline{
    display: flex;
    justify-content: flex-start;
    gap: 2rem;
    align-items: center;
  }

  .bullet{
    width: 20%;
    height: 100%;

    font-family: Open Sans;

    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: space-between;
  }
</style>
