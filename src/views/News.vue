<template>
  <div id="app">
    <News />
  </div>
</template>

<script>
import News from '@/components/News.vue';

export default {
  name: 'NewsPage',
  components: {
    News
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;900&display=swap');

body {
  font-family: 'Roboto';
}

</style>
