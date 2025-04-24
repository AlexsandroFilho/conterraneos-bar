<template>

<section class="contact py-5 bg-light">
    <div class="container">
      <h2 class="text-center mb-4 fw-bold">Entre em Contato</h2>
      <div class="row align-items-center">
        
            <!-- Contato via WhatsApp -->
            <div class="col-md-6 text-center mb-4 mb-md-0">
            <p class="lead">Fale com a gente pelo WhatsApp:</p>
            <a 
                href="https://wa.me/5513982135251" 
                target="_blank" 
                class="btn btn-success btn-lg">
                <i class="bi bi-whatsapp me-2"></i> Chamar no WhatsApp
            </a>
            </div>

            <!-- Mapa de Localização -->
            <div class="col-md-6">
            <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3644.180601804659!2d-46.509329823719035!3d-24.024695678779526!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94ce1f65872edc95%3A0x3121392efc526c57!2sAv.%20Rocha%20Pita%2C%2054%20-%20Jardim%20Trevo%2C%20Praia%20Grande%20-%20SP%2C%2011714-440!5e0!3m2!1spt-BR!2sbr!4v1745454772963!5m2!1spt-BR!2sbr" 
                width="100%" 
                height="300" 
                style="border:0;" 
                allowfullscreen="" 
                loading="lazy"
                referrerpolicy="no-referrer-when-downgrade">
            </iframe>
            </div>

      </div>
    </div>
  </section>

</template>

<script>
    export default {
    name: "Contact"
    };
</script>

<style scoped>
    .contact {
    background-color: #fff8f0;
    }
</style>