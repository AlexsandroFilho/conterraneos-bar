<template>
    <section class="hero d-flex flex-column justify-content-center align-items-center text-center text-white">
      <div class="overlay"></div>
      <div class="content position-relative z-1">
        <h1 class="display-4 fw-bold">Conterrâneo's Bar</h1>
        <p class="lead">Tradição, sabor e aquele jeitinho do sertão!</p>
        <button class="btn btn-primary mt-3" @click="scrollToMenu">Ver cardápio</button>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: "HeroSection",
    methods: {
      scrollToMenu() {
        const section = document.getElementById("menu");
        section?.scrollIntoView({ behavior: "smooth" });
      },
    },
  };
  </script>
  
  <style scoped>
  .hero {
    background-image: url('/assets/fundo.png'); 
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    height: 100vh;
    position: relative;
    color: #F4F4F4;
  }
  
  .overlay {
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    background-color: rgba(35, 32, 32, 0.6); 
    z-index: 0;
  }
  
  .content {
    z-index: 1;
  }

  h1, p {
  color: #F4F4F4;
}

  </style>
  