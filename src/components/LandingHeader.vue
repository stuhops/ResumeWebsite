<template>
  <div
    id="main-container"
    :style="{ backgroundImage: 'url(' + background_image + ')' }"
  >
    <div class="container">
      <h1 id="header-text">Full-Stack<br />Developer.</h1>
      <div class="links">
        <a href="mailto:stuart.hops@gmail.com">
          <button class="outlined-button-light">Contact Me Today</button>
        </a>
        <a id="resume" href="/resume.pdf" download>
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
  margin: 0;
}

#main-container {
  max-width: 100vw;
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
