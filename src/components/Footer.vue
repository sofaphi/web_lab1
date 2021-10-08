<template>
  <footer>
    <div class="ear ear1"></div>
    <div class="ear ear2"></div>
    <div>
      <p>Терентьева 201-322</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>
footer {
  position: relative;
  padding-top: 100px;
  margin-top: 20px;
}

.ear {
  position: absolute;
  width: 100px;
  height: 100px;
}

.ear1 {
  top: 26px;
  left: 0;
  background: url('../assets/ears.png');
  background-size: 317px;
  transform: rotate(13deg);
}

.ear2 {
  top: 23px;
  right: 0;
  background: url('../assets/ears.png');
  background-size: 317px;
  transform: rotate(-8deg);
  background-position: 155px;
}

footer div {
  background: #000;
  padding: 15px;
  color: #fff;
}
</style>