<template>

    <section class="about about-sectionoo py-5">
        <div class="container text-center">
            <div class="about-card p-4 rounded">
                <h2 class="display-5 fw-bold">Conheça o Conterrâneo's Bar</h2>
                <p class="lead">
                    Um pedacinho do sertão no coração da cidade! Com ambiente rústico e acolhedor,
                    o Conterrâneo's Bar oferece sabores únicos, das comidas tradicionais do nordeste e aquele clima de bar do sertão.
                </p>
            </div>    
          
        </div>
      </section>
    
    </template>
    
    <script>
    export default {
      name: "About",
    };
    </script>
    
    <style scoped>
        .about {
        background-image: url('/assets/about2.png');
        background-size: contain;
        background-position: center; 
        height: 500px; 
        }

        .about-section {
            background-color: #F4F4F4;
        }

        .about-card {
            background-color: rgba(255, 255, 255, 0.8); /* leve transparência */
            color: #3A3535;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
        }


    </style>