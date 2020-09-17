<template>
  <div id="main-container">
    <div id="secondary-container">
      <div id="statement">
        <h2>{{ headline }}</h2>
        <p>{{ description }}</p>
      </div>
      <div id="image-section">
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_roll"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_roll"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_roll"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_roll"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_roll"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_roll"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_roll"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_roll"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_roll"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_roll"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Image1x1 from "@/components/Image1x1.vue";

import image_kayak_roll from "@/assets/img/landing-page/kayak-roll.jpg"

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
    Image1x1
  },
  data: function() {
    return {
      image_kayak_roll: image_kayak_roll
    }
  }
};
</script>

<style scoped>
* {
  color: #202020;
}

h2 {
  font-size: clamp(48px, 3vw, 72px);
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

#image-section {
  width: 100%;
  margin: 5vh 0 0 0;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  flex-wrap: wrap;
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
  align-content: stretch;
  align-items: center;
}

#secondary-container {
  flex: 1;
  max-width: 1396px;
  margin: 5vh 10vw 5vh 10vw;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  flex-wrap: no-wrap;
}

#statement {
  flex: 1;
}

.image-flex {
  flex: 1;
  flex-basis: 20%;
  min-width: 105px;
  padding: 8px;
}

@media (max-width: 680px) {
  .image-flex {
    flex-basis: 50%;
  }
}
</style>
