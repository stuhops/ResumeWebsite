<template>
  <div id="main-container">
    <div id="secondary-container">
      <div id="statement">
        <h2 id="header-text" class="flex">{{ headline }}</h2>
        <p class="flex">{{ description }}</p>
      </div>
      <div id="images">
        <img class="image" :src="image1" />
        <img class="image image-low" :src="image2" />
        <img class="image" :src="image3" />
      </div>
      <a id="github" href="https://github.com/stuhops">
        <button class="outlined-button-dark">View GitHub</button>
      </a>
    </div>
  </div>
</template>
<script>
export default {
  name: "TriplePictureStatementSection",
  props: {
    headline: String,
    description: String,
    image1: String,
    image2: String,
    image3: String
  }
};
</script>

<style scoped>
* {
  color: #202020;
}

#content-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

#github {
  max-width: 80vw;
  margin-top: 72px;
}

#header-text {
  flex: 1;
  margin: 0;
}

#images {
  max-width: 1396px;
  width: 95vw;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}

#main-container {
  width: 100vw;
  max-width: 100vw;
  min-height: 130vh;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center top;
  background-color: #f5f5f5;
  display: flex;
  justify-content: center;
  align-items: center;
}

#secondary-container {
  flex: 1;
  max-width: 1396px;
  margin: 25vh 10vw 25vh 10vw;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: column;
  flex-wrap: wrap;
}

#statement {
  max-width: 1396px;
  width: 100%;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  display: flex;
  flex: 1;
}

.flex {
  flex: 1;
}

.image {
  flex: 1;
  max-width: 364px;
  width: 20vw;
  min-width: 100px;
  margin: 14px 3vw 14px 3vw;
}

@media screen and (min-width: 527px) {
  .image-low {
    margin-top: 128px;
  }
}

@media screen and (max-width: 526px) {
  #images {
    flex-direction: column;
  }

  .image {
    flex: 1;
    width: 100%;
  }
}
</style>
