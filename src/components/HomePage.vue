<template>
  <!-- lg:grid-cols-2 -->
  <!-- <div class="grid grid-cols-1  "> -->
  <div class="hero-polygon hero-mask h-screen flex justify-center content-center">
    <div class="flex flex-col justify-center content-center my-auto w-fit">
      <div class="title-text-size1 text-center text-white ">
        Hi 👋🏼
      </div>
      <div class="title-text-size1 text-center text-white">
        <span>I'm </span>
        <span class="bold-theme-text">Ray
          Takemura</span>
      </div>
    </div>
  </div>
  <!-- </div> -->
  <!-- <div class="grid grid-cols-1 h-screen my-auto">
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
  </div> -->
</template>

<script>
export default {
  emits: ['hideLoader'],
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
.hero-mask {
  /* Use "linear-gradient" to add a darken background effect to the image (photographer.jpg). This will make the text easier to read */
  /* background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("./../assets/bamboos2 edited.jpg"); */

  background-image: url("./../assets/texture.svg");
  background-attachment: fixed;
  background-position: center;
  background-repeat: repeat;
  background-size: auto;
  position: relative;

  /* Set a specific height */
  /* height: 100%; */

  /* Position and center the image to scale nicely on all screens */

  /* background-size: 544px 544px, 10px;
  background-repeat: no-repeat, repeat;
  background-position: 100% 100%, 0 0; */
}

.hero-polygon {
  background-image: url("./../assets/Polygon\ 1.svg");
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