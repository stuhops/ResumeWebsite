<template>
  <LandingHeader
    header="Full-Stack\nDeveloper."
    :background_image="LandingHeaderImage"
  />
  <SingleStatementSection
    description="Not only do I like to build great websites, I love to make them look and feel beautiful too. I don't believe a website is complete until the frontend, backend, and documentation are all finished."
    headline="My passion is full-stack web development"
    projectHeadline="Auctionit"
    :projectImage="CodeSnippitImage"
    projectUrl="https://github.com/stuhops/AuctionIt"
  />
  <MyStackSection headline="Let's talk about my stack" />
  <TriplePictureStatementSection
    headline="My Work"
    description="I love working on personal projects and learning new things. Here are some highlights."
    :image1="MoviemaniaImage"
    image1Headline="Movie Mania"
    image1Url="https://github.com/stuhops/cs3200-moviemania-assn4"
    :image2="FroggerImage"
    image2Headline="Frogger"
    image2Url="https://github.com/stuhops/cs5410-frogger-assn4"
    :image3="AuctionitImage"
    image3Headline="AuctionIt"
    image3Url="https://github.com/stuhops/AuctionIt"
  />
  <WorkWithMeSection headline="So you like what you see?\nLet's get together" />
  <PhotoGridSection 
    headline="My life outside of programming" 
    description="Being a good programmer is made easier when you have interests outside of the office. Here is a partial look at my life beyond development."
  />
</template>

<script>
import LandingHeader from "@/components/LandingHeader.vue";
import MyStackSection from "@/components/home/MyStackSection.vue";
import PhotoGridSection from "@/components/home/PhotoGridSection.vue";
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
    PhotoGridSection,
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
