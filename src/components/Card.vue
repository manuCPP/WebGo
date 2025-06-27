<script setup>
import path from '@/assets/images/checkWhite.png'
import path2 from '@/assets/images/closeWhite.png'

import path3 from '@/assets/images/checkGreen.png'
import path4 from '@/assets/images/closeRed.png'



const props = defineProps({
  textVar: String,
  second: {
    type: Boolean,
    default: false
  },
  third: {
    type: Boolean,
    default: false
  },
  price:String,

})

const propsArr = props.textVar.split(',');



</script>

<template>

  <div class="card">
    <h2>{{ price }}</h2>
    <div class="body">
      <div class="line"><div class="imgContainer"><img :src="second? path3 : path" alt=""></div><p>sito a <span>{{ propsArr[0] }}</span> pagine ad alta conversione ottimizzato per dispositivi mobile.</p></div>
      <div class="line"><div class="imgContainer"><img :src="second? path3 : path" alt=""></div><p>Ottimizzazione per motori di ricerca per ottenere piu visite.</p></div>

      <div class="line"><div class="imgContainer"><img :src="second? path3 : path" alt=""></div><p>Integrazione di piattaforme di review per costruire fiducia.</p></div>
      <div class="line"><div class="imgContainer"><img :src="second? path3 : path" alt=""></div><p>Mantenimento e supporto a vita.</p></div>
      <div class="line"><div class="imgContainer"><img :src="second? path3 : path" alt=""></div><p>Cambiamenti gratuiti fino alla completa soddisfazione.</p></div>

      <div class="line"><div  class="imgContainer"><img :style="second || third? 'width:100%' : 'width:70%'" :src="second? third? path : path3 : third? path : path2" alt=""></div><p>{{ propsArr[1] }} pagine localizzate, pensate per presidiare strategicamente i settori in cui operi.</p></div>
      <div class="line"><div class="imgContainer"><img :style="third? 'width:100%' : 'width:70%'" :src="second? third? path : path4 : third? path : path2" alt=""></div><p>10 pagine progetto dedicate ai tuoi lavori precedenti.</p></div>
    </div>
  </div>

</template>

<style scoped>
  img{
    width: 100%;

  }

  .body{
    width: 100%;
    height: 70%;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
  }

  .imgContainer{
    width: 10%;
    display: flex;
    justify-content: center;
    align-items: center;


  }

  .line{
    display: flex;
    justify-content: space-between;
    align-items: center;

    width: 100%;

  }

  .card{
    width: 30%;
    height: 85%;
    border-radius: 1rem;
    border: solid 2px rgb(255, 255, 255);
    box-shadow: 4px 4px 4px #25781e;
    display: flex;
    justify-content: center;
    gap: 2rem;
    align-items: center;
    flex-direction: column;

    padding-inline: 2rem;



  }

  h2{
    display: flex;
    align-items: center;
    justify-content: center;

    width: 100%;
    height: 10%;


    font-family: Onest, sans-serif;
    font-size: 4rem;
    font-weight: 800;
    color: white;
  }

  p{
    width: 85%;
    color: white;
    text-wrap: no-wrap;
    text-align: left;

    font-family: Inter;
    font-weight: 400;
    font-size: 0.8rem;


  }

  .card:nth-child(2){
    background-color: white;
    p, h2{
      color: black;
    }

    border: solid 2px black;
  }
</style>
