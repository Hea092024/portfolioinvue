<template>
  <div id="app">
    <header>
      <h1>My Portfolio</h1>
    </header>
    <main>
      <About />
      <Projects />
      <Contact />
    </main>
  </div>
</template>

<script>
import About from './components/About.vue';
import Contact from './components/Contact.vue';
import Projects from './components/Projects.vue';

export default {
  name: 'App',
  components: {
    About,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>