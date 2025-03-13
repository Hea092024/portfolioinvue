<template>
     <section id="contact" class="contact-page">
      <div class="contact-container">
        <h2>Contact Me</h2>
        <div class="contact-details">
          <div class="contact-info">
            <h3>Hector Acevedo</h3>
            <div class="contact-item">
              <i class="fas fa-envelope"></i>
              <span>ilalo1983@gmail.com</span>
            </div>
            <div class="contact-item">
              <i class="fas fa-phone"></i>
              <span>+47 93 46 22 76 </span>
            </div>
            <div class="contact-item">
              <i class="fas fa-map-marker-alt"></i>
              <span>Bergen, Norway</span>
            </div>
          </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
  name: 'ContactPage', 
};
</script>

<style scoped>
h2 {
  color: #42b983;
}

.contact-page {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 5rem 5%;
}
</style>
