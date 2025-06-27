<script setup>

</script>


<template>
  <main class="clipped">
    <div class="container">
      <div class="texts">
        <h1>Siti web professionali per tutti</h1>
        <p>Design moderno, funzionalità avanzate e prezzi che si adattano a te. Perché un buon sito non deve essere un lusso.</p>
        <button>Contattami</button>
      </div>

      <div style="z-index: 100;" class="imgDiv">
        <img style="z-index: 100;" src="@/assets/images/pc.svg" alt="Immagine di un pc">
      </div>
    </div>
  </main>
  <div class="custom-shape-divider-bottom-1750537445">
    <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
        <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" class="shape-fill"></path>
    </svg>
  </div>

</template>

<style scoped>



.custom-shape-divider-bottom-1750537445 {
    position: relative;
    bottom: 0;
    background-color: red;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
    transform: rotate(180deg);
}

.custom-shape-divider-bottom-1750537445 svg {
    position: relative;
    display: block;
    background-color: var(--primary-color);
    width: calc(100% + 1.3px);
    height: 142px;
}

.custom-shape-divider-bottom-1750537445 .shape-fill {
    fill: #ffffff;
}

  main{
    background-color: var(--primary-color);
    width: 100%;
    height: 50vh;

    display: flex;
    justify-content: center;
    align-items: center;
  }

  button{
    background-color: white;
    color: rgb(21, 21, 36);
    width: 20vh;
    height: 6.5vh;
    border: none;
    border-radius: 2rem;
    font-family: Inter;
    font-size: 1.2rem;
    font-weight: 500;
    transition: all 0.3s ease-in-out;
  }



  .container{
    width: 75%;
    height: 100%;

    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .imgDiv{
    width: 50%;
    height: 100%;

    animation: Float infinite ease-in-out 2s;
  }

  .texts{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    gap: 3rem;

    width: 50%;
    height: 100%;
    h1{
      font-family: Open Sans;
      font-weight: 600;
      font-size: 4rem;
      color: white;
    }
    p{
      text-wrap: wrap;
      font-size: 1.1rem;
      color: white;
      font-family: Inter;
      line-height: 150%;
      width: 80%;
    }


    button:hover{
      transform: scale(1.05);
      color: var(--primary-color);
      cursor: pointer;
    }
  }




  @keyframes Float {
  0% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-20px);
  }
  100% {
    transform: translateY(0px);
  }
  }




  @media screen and (max-width: 1420px){
    main{
      height: 65vh;

    }

    .container{
      width: 95%;
    }
  }
</style>
