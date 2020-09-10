<template>
  <LandingHeader
    header="Full-Stack\nDeveloper."
    :background_image="LandingHeaderImage"
  />
  <SingleStatementSection
    headline="My passion and focus is Full-Stack web development"
  />
</template>

<script>
import LandingHeader from "@/components/LandingHeader.vue";
import SingleStatementSection from "@/components/SingleStatementSection.vue";

import LandingHeaderImage from "@/assets/img/landing-page/welcome.jpg";

export default {
  name: "Home",
  components: {
    LandingHeader,
    SingleStatementSection
  },
  data: function() {
    return {
      LandingHeaderImage: LandingHeaderImage
    };
  }
};
</script>
