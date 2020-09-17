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
          :image="image_bridge_mtn"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_kayak_braden"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_lp_wall"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_ski_laugh"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_many_pools"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_lp_base"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_ski_pow"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_touchstone"
        />
        <Image1x1 
          class="image-flex" 
          :image="image_west_rim"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Image1x1 from "@/components/Image1x1.vue";

import image_kayak_roll from "@/assets/img/landing-page/photo-grid/kayak-roll.jpg";
import image_bridge_mtn from "@/assets/img/landing-page/photo-grid/bridge-mtn.jpg";
import image_kayak_braden from "@/assets/img/landing-page/photo-grid/kayak-braden.jpg";
import image_lp_base from "@/assets/img/landing-page/photo-grid/lone-peak-base.jpg";
import image_lp_wall from "@/assets/img/landing-page/photo-grid/lone-peak-wall.jpg";
import image_many_pools from "@/assets/img/landing-page/photo-grid/many-pools.jpg";
import image_ski_laugh from "@/assets/img/landing-page/photo-grid/ski-laugh.jpg";
import image_ski_pow from "@/assets/img/landing-page/photo-grid/ski-pow.jpg";
import image_touchstone from "@/assets/img/landing-page/photo-grid/touchstone.jpg";
import image_west_rim from "@/assets/img/landing-page/photo-grid/west-rim.jpg";

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
      image_kayak_roll: image_kayak_roll,
      image_bridge_mtn: image_bridge_mtn,
      image_kayak_braden: image_kayak_braden,
      image_lp_base: image_lp_base,
      image_lp_wall: image_lp_wall,
      image_many_pools: image_many_pools,
      image_ski_laugh: image_ski_laugh,
      image_ski_pow: image_ski_pow,
      image_touchstone: image_touchstone,
      image_west_rim: image_west_rim
    }
  }
};
</script>

<style scoped>
* {
  color: #202020;
}

h2 {
  margin-bottom: 8px;
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
  text-align: center
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
