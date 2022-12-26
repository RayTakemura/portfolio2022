<template>
  <!-- lg:grid-cols-2 -->
  <div class="grid grid-cols-1  h-screen ">
    <div class="grid grid-cols-1 justify-center content-center mt-auto lg:mt-0 ">
      <div class="title-text-size1 text-center text-white">
        Hi 👋🏼
      </div>
      <div class="title-text-size1 text-center text-white ">
        <span>I'm </span>
        <span class="bold-theme-text">Ray
          Takemura</span>
      </div>
    </div>
    <!-- <div class="container m-auto lg:ml-14" id="wrap">
      <iframe class="responsive-iframe" id="scaled-frame"
        src='https://my.spline.design/untitled-e0a1d03472edbe77f3631bf8d12c4d28/' frameborder='0'></iframe>
    </div> -->
    <!-- <div class="container m-auto lg:ml-14" id="wrap">
      <iframe class="responsive-iframe" id="scaled-frame"
        src='https://my.spline.design/untitled-e0a1d03472edbe77f3631bf8d12c4d28/' frameborder='0'></iframe>
    </div> -->
  </div>
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
    let logo = document.querySelector('#scaled-frame');

    logo.addEventListener('load', (event) => {
      setTimeout(() => {
        //TODO: emit an event to App.vue so that we can get rid of the initial loading screen!
        console.log('Logo has been loaded!', event);
        this.$emit("hideLoader")
      }, 2000);

    });
  }
}
</script>

<style scoped >
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