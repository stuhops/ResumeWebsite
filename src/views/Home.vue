<template>
  <LandingHeader
    header="Full-Stack\nDeveloper."
    :background_image="LandingHeaderImage"
  />
</template>

<script>
import LandingHeader from "@/components/LandingHeader.vue";

import LandingHeaderImage from "@/assets/img/landing-page/welcome.jpg";

export default {
  name: "Home",
  components: {
    LandingHeader
  },
  data: function() {
    return {
      LandingHeaderImage: LandingHeaderImage
    };
  }
};
</script>
