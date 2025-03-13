<template>
  <div id="app">
    <header>
      <h1>My Portfolio</h1>
    </header>
    <main>
      <MainPage />
      <MyProjects />
      <ContactPage />
      <AboutPage />
    </main>
  </div>
</template>

<script>
import MainPage from './components/MainPage.vue';
import AboutPage from './components/AboutPage.vue';
import ContactPage from './components/ContactPage.vue';
import MyProjects from './components/MyProjects.vue';

export default {
  name: 'App',
  components: {
    MainPage,
    AboutPage,
    ContactPage,
    MyProjects
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