<template>
  <main>
    <h1>News</h1>
    <div>
      <div class="article-block" v-for="(article, index) in news" :key="index">
        <h2><router-link :to='"/article/" + article.id'>{{article.id}} {{article.name}}</router-link></h2>
        <p>{{article.date}}</p>
        <p>{{article.shortDesc}}</p>
      </div>
    </div>
  </main>
</template>

<script>
import news from '../assets/articles.json'

export default {
  name: 'News',
  data(){
      return {
        news
    };
  }
}
</script>

<style scoped>
.article-block {
    margin-bottom: 20px;
    padding: 8px;
    background: #e2e1e2;
    border-radius: 8px;
}

a {
  color: #000;
}
a:hover {
  text-decoration: underline;
}
</style>