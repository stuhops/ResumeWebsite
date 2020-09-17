<template>
  <div id="main-container">
    <div id="secondary-container">
      <div id="image-container">
        <Image4x3
          id="projectImage"
          :image="projectImage"
          :headline="projectHeadline"
          :url="projectUrl"
        />
      </div>
      <div id="statement">
        <h2>{{ headline }}</h2>
        <p>{{ description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
import Image4x3 from "@/components/Image4x3.vue";

export default {
  name: "SingleStatementSection",
  props: {
    description: String,
    headline: String,
    projectDescription: String,
    projectHeadline: String,
    projectImage: String,
    projectUrl: String
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

#header-text {
  flex: 1;
  margin: 0;
}

#content-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

#image {
  flex: 1;
  width: 100%;
  object-fit: cover;
  position: relative;
}

#image-container {
  flex: 1;
  min-width: 200px;
  width: 20vw;
  max-width: 500px;
  height: 100%;
  margin: 0 5vw 0 0;
}

#main-container {
  max-width: 100vw;
  min-height: 130vh;
  padding: 48px 8px 48px 8px;
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
  margin: 5vh 10vw 5vh 10vw;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
}

#statement {
  flex: 1;
}
</style>
