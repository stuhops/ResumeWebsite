<template>
  <div id="container43">
    <div id="image43" :style="{ backgroundImage: 'url(' + image + ')' }">
      <div id="content43">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Image4x3",
  props: {
    image: String,
    headline: String,
    description: String
  }
};
</script>

<style scoped>
#container43 {
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

#content43 {

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
</style>
