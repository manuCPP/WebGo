<script setup>
import Card from '@/components/Card.vue'
</script>


<template>
  <div class="greenContainer">
    <div class="container">
      <Card textVar="5" price="$299" />
      <Card second="true" textVar="10, 10" price="$399"/>
      <Card third="true" textVar="15, 20" price="$499"/>
    </div>
  </div>
</template>

<style scoped>
  .greenContainer{
    width: 100%;
    height: 80vh;

    background-color: var(--primary-color);

    display: flex;
    justify-content: center;
    align-items: center;
  }

  .container{
    width: 95%;
    height: 100%;

    display: flex;
    align-items: center;
    justify-content: space-between;
  }



</style>
