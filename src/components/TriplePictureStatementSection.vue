<template>
  <div id="main-container">
    <div id="secondary-container">
      <div id="statement">
        <h2 id="header-text" class="flex">{{ headline }}</h2>
        <p class="flex">{{ description }}</p>
      </div>
      <div id="images">
        <Image4x3
          class="image" 
          :image="image1"
          :headline="image1Headline"
          :url="image1Url"
        />
        <Image4x3
          class="image image-low" 
          :image="image2"
          :headline="image2Headline"
          :url="image2Url"
        />
        <Image4x3
          class="image" 
          :image="image3"
          :headline="image3Headline"
          :url="image3Url"
        />
      </div>
      <a id="github" href="https://github.com/stuhops">
        <button class="outlined-button-dark">View GitHub</button>
      </a>
    </div>
  </div>
</template>

<script>
import Image4x3 from "@/components/Image4x3.vue";

export default {
  name: "TriplePictureStatementSection",
  props: {
    headline: String,
    description: String,
    image1: String,
    image1Headline: String,
    image1Url: String,
    image2: String,
    image2Headline: String,
    image2Url: String,
    image3: String,
    image3Headline: String,
    image3Url: String
  },
  components: {
    Image4x3
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
