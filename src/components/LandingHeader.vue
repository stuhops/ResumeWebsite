// TODO: Make #header-text take the prop header and break on a new line
<template>
  <div class="main-container" :style="{ backgroundImage: 'url(' + background_image + ')' }">
    <div class="container">
      <h1 id="header-text">Full-Stack<br />Developer.</h1>
      <div class="links">
        <a>
          <button class="outlined-button-light">Contact Me Today</button>
          <button class="borderless-button-light">Download Resume</button>
        </a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "LandingHeader",
  props: {
    background_image: String,
    header: String
  }
};
</script>

<style scoped>
#header-text {
  flex: 1;
  font-size: clamp(72px, 8vw, 120px);
  margin: 0;
}

.main-container {
  width: 100vw;
  height: 100vh;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center top;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

.container {
  max-width: 1396px;
  margin: 5vh 10vw 5vh 10vw;
}
</style>
