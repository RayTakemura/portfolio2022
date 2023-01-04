<template>
  <!-- lg:grid-cols-2 -->
  <div class="grid grid-cols-1 h-screen ">
    <div class="hero-image my-auto">
      <div class="grid grid-cols-1 justify-center content-center my-auto ">
        <div class="title-text-size1 text-center text-white">
          Hi 👋🏼
        </div>
        <div class="title-text-size1 text-center text-white ">
          <span>I'm </span>
          <span class="bold-theme-text">Ray
            Takemura</span>
        </div>
      </div>
    </div>
    <ViewPort />
  </div>
</template>

<script>
import ViewPort from "./ViewPort.vue"
export default {
  emits: ['hideLoader'],
  component: {
    ViewPort,
  },
  methods: {
    loadImage() {
      alert("Image is loaded");
    }
  },
  mounted() {
  }
}
</script>

<style scoped >
.hero-image {
  /* Use "linear-gradient" to add a darken background effect to the image (photographer.jpg). This will make the text easier to read */
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("./../assets/bamboos2\ edited.jpg");

  /* Set a specific height */
  height: 100%;

  /* Position and center the image to scale nicely on all screens */
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}



#wrap {
  width: 23rem;
  height: 23rem;
  padding: 0;
  overflow: hidden;
}

#scaled-frame {
  width: 80rem;
  height: 80rem;
  border: 0px;
}

/* zoom: 0.5; */
/* width: 350%;
  height: 100vh; */
#scaled-frame {

  -webkit-transform: scale(0.3);
  -webkit-transform-origin: 0 0;
  -o-transform: scale(0.3);
  -o-transform-origin: 0 0;
  -moz-transform: scale(0.3);
  -moz-transform-origin: 0 0;
}

@media screen and (-webkit-min-device-pixel-ratio:0) {
  #scaled-frame {
    zoom: 1;
  }
}

@media screen and (min-width: 1024px) {
  #scaled-frame {
    zoom: 1;
    -moz-transform: scale(0.3);
    -o-transform: scale(0.3);
    -webkit-transform: scale(0.3);

  }
}
</style>