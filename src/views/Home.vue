<template>
  <LandingHeader
    header="Full-Stack\nDeveloper."
    :background_image="LandingHeaderImage"
  />
  <SingleStatementSection
    :image="CodeSnippitImage"
    headline="My passion is full-stack web development"
    description="Not only do I like to build great websites, I love to make them look and feel beautiful too. I don't believe a website is complete until the frontend, backend, and documentation are all finished."
  />
  <MyStackSection
    headline="Let's talk about my stack"
  />
  <TriplePictureStatementSection
    headline="My Work"
    description="I love working on personal projects and learning new things. Here are some highlights."
    :image1="MoviemaniaImage"
    :image2="FroggerImage"
    :image3="AuctionitImage"
  />
  <WorkWithMeSection
    headline="So you like what you see?\nLet's get together"
  />
</template>

<script>
import LandingHeader from "@/components/LandingHeader.vue";
import MyStackSection from "@/components/home/MyStackSection.vue"
import SingleStatementSection from "@/components/SingleStatementSection.vue";
import TriplePictureStatementSection from "@/components/TriplePictureStatementSection.vue";
import WorkWithMeSection from "@/components/WorkWithMeSection.vue";

import AuctionitImage from "@/assets/img/landing-page/auctionit_signup.png";
import CodeSnippitImage from "@/assets/img/landing-page/code_snippit43.png";
import FroggerImage from "@/assets/img/landing-page/frogger.png";
import LandingHeaderImage from "@/assets/img/landing-page/welcome.jpg";
import MoviemaniaImage from "@/assets/img/landing-page/moviemania.png";
import SingleStatementImage from "@/assets/img/landing-page/project-grid.jpg";

export default {
  name: "Home",
  components: {
    LandingHeader,
    MyStackSection,
    SingleStatementSection,
    TriplePictureStatementSection,
    WorkWithMeSection
  },
  data: function() {
    return {
      AuctionitImage: AuctionitImage,
      CodeSnippitImage: CodeSnippitImage,
      FroggerImage: FroggerImage,
      LandingHeaderImage: LandingHeaderImage,
      MoviemaniaImage: MoviemaniaImage,
      SingleStatementImage: SingleStatementImage
    };
  }
};
</script>
