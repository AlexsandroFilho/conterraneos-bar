<template>
    <section id="menu" class="menu py-5 bg-menu">
        <div class="custom-container">
            <h2 class="text-center text-white mb-4">Nosso Cardápio</h2>
            <div class="row row-cols-1 row-cols-md-3 g-4">
            <div class="col" v-for="item in menuItems" :key="item.id">
                <div class="menu-card h-100">
                <img :src="item.image" class="card-img-top img-custom" :alt="item.name" />
                <div class="card-body">
                    <h5 class="card-title">{{ item.name }}</h5>
                    <p class="card-text">{{ item.description }}</p>
                    <p class="text-muted"><strong>R$ {{ item.price.toFixed(2) }}</strong></p>
                </div>
                </div>
            </div>
            </div>
        </div>
</section>

</template>

<script>

export default {
  name: "Menu",
  data() {
    return {
      menuItems: [
        {
          id: 1,
          name: "Contra-filé com fritas",
          description: "Refeição com arroz, feijão carioca, batata frita e contra-filé.",
          price: 35.00,
          image: "/assets/ccontraFile.jpeg",
        },
        {
          id: 2,
          name: "Vaca atolada",
          description: "Refeição com arroz, feijão carioca, e vaca atolada.",
          price: 30.00,
          image: "/assets/vaca.jpeg",
        },
        {
          id: 3,
          name: "Filé de frango",
          description: "Refeição com arroz, feijão carioca, e filé de frango.",
          price: 30.00,
          image: "/assets/baiao.png",
        },
        {
          id: 4,
          name: "Calabresa acebolada",
          description: "Refeição com arroz, feijão carioca, e calabresa acebolada.",
          price: 25.00,
          image: "/assets/baiao.png",
        },
        {
          id: 5,
          name: "Filé de peixe",
          description: "Refeição com arroz, feijão carioca, e filé de peixe.",
          price: 38.00,
          image: "/assets/baiao.png",
        },
        {
          id: 6,
          name: "Mocotó",
          description: "Refeição com arroz, feijão carioca, e mocotó.",
          price: 30.00,
          image: "/assets/baiao.png",
        },
        {
          id: 7,
          name: "Galinha caipira",
          description: "Refeição com arroz, feijão carioca, e galinha caipira com quiabo.",
          price: 30.00,
          image: "/assets/galinha.jpeg",
        },
        {
          id: 8,
          name: "Carne seca com mandioca frita", 
          description: "Refeição com arroz, feijão carioca, e carne seca com mandioca frita.",
          price: 35.00,
          image: "/assets/carneSeca.jpeg",
        },
        {
          id: 9,
          name: "Bisteca com ovo",
          description: "Refeição com arroz, feijão carioca, e bisteca com ovo.",
          price: 25.00,
          image: "/assets/baiao.png",
        },
      ],
    };
  },
};


</script>

<style scoped>
    .img-custom {
        height: 250px;
        object-fit: cover;
        border-radius: 0.5rem;
        border-bottom: #3A3535 2px solid;
        padding: 5px;
    }

    .bg-menu {
        background-color: #232020;
    }

    .custom-container {
        max-width: 900px;
        margin: 0 auto;
    }

    .menu-card{
        max-width: 320px;
        margin: 0 auto;
        padding: 5px;
        border: 2px solid #FF7315;
        border-radius: 0.5rem;
        background-color: white;
      }

    .card-text{
        padding-bottom: 10px;
        color: #3A3535;
        border-bottom: #3A3535 2px solid;
    }

    @media (max-width: 576px) {
        .img-custom {
            height: 200px;
        }
        .menu-card {
            max-width: 90%;
            font-size: 0.9rem;
            padding: 0.75rem;
        }
    }

</style>