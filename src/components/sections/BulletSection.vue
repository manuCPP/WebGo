<script setup>
import Bullet from '../Bullet.vue'
import Spacers from '../Spacer.vue'
</script>


<template>
  <main>
    <h1>Perche scegliere WebGo</h1>
    <div class="container">
      <Bullet img="customer-service.png" title="Servizi offerti" body="Dal design alla pubblicazione, creiamo siti veloci, intuitivi e ottimizzati per la tua attività."/>
      <Bullet img="best-price.png" title="Prezzi convenienti" body="Soluzioni web professionali a prezzi accessibili, ideali per startup, freelance e piccole imprese."/>
      <Bullet img="clock.png" title="Contatto rapido" body="Hai un'idea? Scrivici e in pochi giorni avrai un sito pronto per il tuo business."/>
    </div>
  </main>
</template>


<style scoped >

main{
  height: 40vh;
  width: 75%;

  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}

.container{
  width: 100%;
  height: 8rem;
  display: flex;
  justify-content: space-between;


}

h1{
  font-family: Open Sans;
  font-size: 2.5rem;
}


@media screen and (max-width: 1420px){
  main{
    width: 95%;
  }
}

</style>
