<template>
  <div>
    <h2>Hector's Portfolio</h2>
    <!-- Navigation -->
    <nav class="navbar">
      <a href="#home" class="logo">Hector's Portfolio</a>
      <div class="hamburger" @click="toggleNav">
        <i class="fas fa-bars"></i>
      </div>
      <ul class="nav-links" :class="{ active: isNavActive }">
        <li><a href="#home" @click="scrollToSection('#home')">Home</a></li>
        <li><a href="#skills" @click="scrollToSection('#skills')">Skills</a></li>
        <li><a href="#projects" @click="scrollToSection('#projects')">Projects</a></li>
        <li><a href="contact.html">Contact</a></li>
        <li><a href="aboutme.html">About Me</a></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'MainPage',
  data() {
    return {
      // State to track whether the nav is active or not
      isNavActive: false
    };
  },
  methods: {
    toggleNav() {
      // Toggle the value of isNavActive
      this.isNavActive = !this.isNavActive;
    },
    scrollToSection(target) {
      const section = document.querySelector(target);
      if (section) {
        section.scrollIntoView({
          behavior: 'smooth',
          block: 'start'
        });
      }
    }
  }
};
</script>

<style scoped>
h2 {
  color: #42b983;
}

/* Add styles for active state of nav-links if needed */
.nav-links.active {
  /* Example: slide down the nav menu */
  display: block;
}
</style>
