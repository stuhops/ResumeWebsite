<template>
  <div id="container11">
    <div id="image11" :style="{ backgroundImage: 'url(' + image + ')' }">
      <div v-if="url || headline" id="content11">
        <div id="content-container11">
          <h3 v-if="headline" id="headline11">{{ headline }}</h3>
          <a v-if="url" id="button11" :href="url">
            <button class="outlined-button-light">View Project</button>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Image1x1",
  props: {
    headline: String,
    image: String,
    url: String
  }
};
</script>

<style scoped>
#button11 {
  margin: 0;
}

#container11 {
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

#content11 {
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

#content-container11 {
  display: flex;
  background-color: rgba(0, 0, 0, 0.5);
  flex: 1;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}


@media (hover: hover) {
  #content-container11 {
    visibility: hidden;
    opacity: 0;
    transition: visibility 0s linear 0.5s, opacity 0.5s linear;
  }

  #image11:hover #content-container11 {
    visibility: visible;
    opacity: 1;
    transition-delay: 0s;
  }
}

@media (hover: none) {
  #content-container11 {
    visibility: visible;
  }
}

#headline11 {
  margin: 8px 0 8px 0;
  text-shadow: 0px 0px 10px #000000;
  text-shadow: 0px 0px 10px #000000;
}

#image11 {
  flex: 1;
  width: 100%;
  object-fit: cover;
  padding: 100% 0 0 0;
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
