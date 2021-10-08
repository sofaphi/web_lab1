<template>
  <header>
    <div class="logo">LOGO</div>
    <nav>
      <p><router-link to="/">Main</router-link></p>
      <p><router-link to="/news">News</router-link></p>
    </nav>
  </header>
</template>

<script>

export default {
  name: 'Header'
}
</script>

<style scoped>
  header {
    font-family: 'Roboto';
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #000;
    color: #fff;
    padding: 7px 20px;
    background-image: url('../assets/mustache.png');
    background-size: 150px 60px;
    background-repeat: no-repeat;
    background-position: center;
  }
  
  nav {
    display: flex;
  }
  
  p {
    margin-right: 25px;
  }
  
  p:last-child {
    margin-right: 0;
  }
  
  a {
    text-decoration: none;
    color: #fff;
  }
  a:hover {
    font-weight:700;
  }
</style>