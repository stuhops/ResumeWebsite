<template>
  <div id="container43">
    <div id="image43" :style="{ backgroundImage: 'url(' + image + ')' }">
      <div v-if="headline || url" id="content43">
        <div id="content-container43">
          <h3 v-if="headline" id="headline43">{{ headline }}</h3>
          <a v-if="url" id="button43" :href="url">
            <button class="outlined-button-light">View Project</button>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Image4x3",
  props: {
    headline: String,
    image: String,
    url: String
  }
};
</script>

<style scoped>
#button43 {
  margin: 0;
}

#container43 {
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

@media (max-width: 526px) {
  #container43 {
    margin-left: 0;
    margin-right: 0;
  }
}

#content43 {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  display: flex;
  justify-content: center;
  align-content: center;
  z-index: 1;
}

#content-container43 {
  display: flex;
  background-color: rgba(0, 0, 0, 0.5);
  flex: 1;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}


@media (hover: hover) {
  #content-container43 {
    visibility: hidden;
    opacity: 0;
    transition: visibility 0s linear 0.5s, opacity 0.5s linear;
  }

  #image43:hover #content-container43 {
    visibility: visible;
    opacity: 1;
    transition-delay: 0s;
  }
}

@media (hover: none) {
  #content-container43 {
    visibility: visible;
  }
}

#headline43 {
  margin: 8px 0 8px 0;
  text-shadow: 0px 0px 10px #000000;
  text-shadow: 0px 0px 10px #000000;
}

#image43 {
  flex: 1;
  width: 100%;
  object-fit: cover;
  padding: 133% 0 0 0;
  position: relative;
  background-size: contain;
  background-repeat: no-repeat;
}

.flex {
  flex: 1;
  justify-content: center;
  align-content: center;
}
</style>
