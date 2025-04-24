<script setup lang="ts">
  import { defineComponent } from 'vue'
  import Header from './components/Header.vue'
  import HeroSection from './components/HeroSection.vue'
  import About from './components/About.vue'
  import Menu from './components/Menu.vue'
  import Contact from './components/Contact.vue'
  import Footer from './components/Footer.vue' 
 

</script>

<template>
<div id="app">
    <Header />
    
    <main>
      <HeroSection />
      <div class="section-divider"></div>
      <About />
      <div class="section-divider"></div>
      <Menu />
      <div class="section-divider"></div>
      <Contact />
      <Footer />
    </main>
</div>
</template>

<style scoped>
  body {
    font-family: 'Segoe UI', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #fff;
  }
  main {
    padding: 2rem 1rem;
    }


  :root {
    --cor-fundo: #F4F4F4;
    --cor-destaque: #FF7315;
    --cor-texto-principal: #232020;
    --cor-texto-secundario: #3A3535;
  }

  body {
    background-color: var(--cor-fundo);
    color: var(--cor-texto-principal);
    font-family: 'Arial', sans-serif;
  }

  h1, h2, h3, h4 {
    color: var(--cor-texto-principal);
  }

  p, span, a {
    color: var(--cor-texto-secundario);
  }

  .btn-warning {
    background-color: var(--cor-destaque);
    border-color: var(--cor-destaque);
    color: white;
  }

  .btn-warning:hover {
    background-color: #e06613;
    border-color: #e06613;
  }
</style>