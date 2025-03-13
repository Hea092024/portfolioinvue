<template>
  <div>
    <h2>My Projects</h2>
  </div>

   <!-- Navigation -->
  <nav class="navbar">
    <a href="#home" class="logo">Hector`s Portfolio</a>
    <div class="hamburger" onclick="toggleNav()">
      <i class="fas fa-bars"></i>
    </div>
    <ul class="nav-links">
      <li><a href="#home">Home</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="contact.html">Contact</a></li>
      <li><a href="aboutme.html">About Me</a></li>
    </ul>
  </nav>

    <!-- Hero Section -->
  <section id="home" class="hero">
    <div class="hero-content">
      <h1>Frontend Developer</h1>
      <p>
        Building digital experiences that merge creativity with technology
      </p>
      <p class="higlight">Specializing in modern web development</p>
      <a href="contact.html" class="cta-button">Let`s Connect</a>
    </div>
    <div class="hero-image">
      <img src="../assets/logo.png" alt="Profile" class="profile-img" />
    </div>
  </section>
</template>

<script>
export default {
  name: 'MyProjects', 
};
</script>

<style scoped>
h2 {
  color: #42b983;
}
</style>
