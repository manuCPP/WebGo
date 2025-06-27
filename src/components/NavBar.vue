<script setup>
import { RouterLink } from 'vue-router';
</script>


<template>
  <nav>
    <h1>WebGo</h1>
    <div class="links">
        <RouterLink class="navLink">Home</RouterLink>
        <RouterLink class="navLink">Noi</RouterLink>
        <RouterLink class="navLink">Lavori</RouterLink>
        <RouterLink class="navLink">Contattami</RouterLink>
    </div>
  </nav>

</template>

<style scoped>
  nav{
    width: 75%;
    height: 15vh;

    display: flex;
    justify-content: space-between;
    align-items: center;

    font-family: Open Sans;
    color: black;
  }

  h1{
    font-size: 2.2rem;
    font-weight: 500;
  }

  .navLink{
    text-decoration: none;
    color: black;
    font-size: 1.2rem;
    font-weight: 400;
    font-family: Inter;

    transition: all 0.3s ease-in-out;
  }

  .navLink:nth-child(4){
    background-color: var(--primary-color);
    border-radius: 2rem;
    color: white;
    padding-inline: 2rem;
    padding-block: 1rem;
  }

    .navLink:hover{
    transform: scale(1.05);
    color: rgb(77, 225, 37);

  }

  .navLink:nth-child(4):hover{
    color: rgb(255, 255, 255);
    background-color: rgb(45, 170, 45);
  }

  .links{
    width: 35%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  @media screen and (max-width: 1420px){    /* Prima media query per i mac o portatili*/
    nav{
      width: 95%;

    }
  }
</style>
