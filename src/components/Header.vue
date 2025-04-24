<template>
    <header class="navbar navbar-expand-lg navbar-dark bg-dark sticky-top">
        <div class="container">
            <a class="navbar-brand" href="#">Conterrâneo's Bar</a>
            <button
                class="navbar-toggler"
                type="button"
                data-bs-toggle="collapse"
                data-bs-target="#navbarNav"
                >
                <span class="navbar-toggle-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="">Inicio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="">Sobre</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="">Cardápio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="">Contato</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script lang="ts" >
import { defineComponent } from 'vue'
export default defineComponent({
    name: 'Header'
})


</script>