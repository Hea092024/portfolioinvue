<template>
  <div>
    <h2>Hector's Portfolio</h2>
    <nav class="navbar">
      <a href="#home" class="logo">Hector's Portfolio</a>
      <div class="hamburger" @click="toggleNav">
        <i class="fas fa-bars"></i>
      </div>
      <ul class="nav-links" :class="{ active: isNavActive }">
        <li><a href="#home" @click="navigateTo('home')">Home</a></li>
        <li><a href="#skills" @click="navigateTo('skills')">Skills</a></li>
        <li><a href="#projects" @click="navigateTo('projects')">Projects</a></li>
        <li><a href="contact.html" @click="navigateTo('contact')">Contact</a></li>
        <li><a href="aboutme.html" @click="navigateTo('about')">About Me</a></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'MainPage',
  data() {
    return {
      isNavActive: false
    };
  },
  methods: {
    toggleNav() {
      this.isNavActive = !this.isNavActive;
    },
    navigateTo(page) {
      this.$emit('update-page', page);  // Emit the page name to the parent to update activePage
    }
  }
};
</script>

<style scoped>
h2 {
  color: #42b983;
}

.nav-links.active {
  display: block;
}
</style>
