<template>
  <LandingHeader
    header="Full-Stack\nDeveloper."
    :background_image="LandingHeaderImage"
  />
  <SingleStatementSection
    :image="SingleStatementImage"
    headline="My passion is full-stack web development"
    description="Not only do I like to build great websites, I love to make them look and feel beautiful too. I don't believe a website is complete until the UX, UI, Frontend, and backend are all complete."
  />
  <TriplePictureStatementSection
    headline="My Work"
    description="I love working on personal projects and learning new things. Here are some highlights."
    :image1="SingleStatementImage"
    :image2="SingleStatementImage"
    :image3="SingleStatementImage"
  />
</template>

<script>
import LandingHeader from "@/components/LandingHeader.vue";
import SingleStatementSection from "@/components/SingleStatementSection.vue";
import TriplePictureStatementSection from "@/components/TriplePictureStatementSection.vue";

import LandingHeaderImage from "@/assets/img/landing-page/welcome.jpg";
import SingleStatementImage from "@/assets/img/landing-page/project-grid.jpg";

export default {
  name: "Home",
  components: {
    LandingHeader,
    SingleStatementSection,
    TriplePictureStatementSection
  },
  data: function() {
    return {
      LandingHeaderImage: LandingHeaderImage,
      SingleStatementImage: SingleStatementImage
    };
  }
};
</script>
