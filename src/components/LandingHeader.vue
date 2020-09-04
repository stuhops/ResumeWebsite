<template>
  <div class="main-container" :style="{ backgroundImage: 'url(' + background_image + ')' }">
    <div class="container">
      <h1 id="header-text">{{ header }}</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "LandingHeader",
  props: {
    background_image: String,
    header: String
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#header-text {
  font-size: clamp(72px, 8vw, 120px);
  white-space: pre-wrap;
}

.main-container {
  width: 100vw;
  height: 100vh;
  background-color: green;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center top;
  display: flex;
  justify-content: center;
}

.container {
  max-width: 1396px;
  margin: 5vh 10vw 5vh 10vw;
}
</style>
