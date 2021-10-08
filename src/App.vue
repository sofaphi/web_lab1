<template>
  <div id="app">
    <div id="nav">
      <Header />
    </div>
    <div class="content">
      <router-view/>
    </div>
    <Footer />
  </div>
</template>

<script>
  import Header from '@/components/Header.vue';
  import Footer from '@/components/Footer.vue';

  export default {
    name: 'App',
    components: {
      Footer,
      Header
    }
  }
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;900&display=swap');

body {
  font-family: 'Roboto';
}

html,
body {
  height: 100%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  min-height: 100%;
  display: flex;
  flex-direction: column;
  max-width: 1000px;
  margin: 0 auto;
}

.content {
  flex: 1 1 auto;
}
</style>
