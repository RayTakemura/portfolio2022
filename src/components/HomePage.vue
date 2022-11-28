<template>
  <div class="grid grid-cols-1 lg:grid-cols-2 ">
    <div class="flex flex-col justify-items-start">
      <div class="text-4xl text-white">
        Hi 👋🏼 I'm
      </div>
      <div class="text-4xl text-white">
        Ray Takemura
      </div>
    </div>
    <div class="container " id="wrap">
      <iframe class="responsive-iframe" id="scaled-frame"
        src='https://my.spline.design/untitled-e0a1d03472edbe77f3631bf8d12c4d28/' frameborder='0'></iframe>

    </div>


    <!-- <div class="border-2 border-red-500">1</div>
    <div class="border-2 border-yellow-500">2</div> -->
  </div>


</template>

<script>
export default {
}
</script>

<style>
/* #wrap {
  width: 100%;
  height: 85vh;
  padding: 0;
  overflow: hidden;
}

#scaled-frame {
  width: 100%;
  height: 85vh;
  border: 0px;
}

#scaled-frame {
  zoom: 1;
  -moz-transform: scale(0.5);
  -moz-transform-origin: 0 0;
  -o-transform: scale(0.5);
  -o-transform-origin: 0 0;
  -webkit-transform: scale(0.5);
  -webkit-transform-origin: 0 0;
}

@media screen and (-webkit-min-device-pixel-ratio:0) {
  #scaled-frame {
    zoom: 1;
  }
}

@media screen and (width < 1024px) {
  #scaled-frame {
    width: 100vw;
    -webkit-transform: scale(0.5);
    -o-transform: scale(0.5);
    -moz-transform: scale(0.5);
  }
} */
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

#scaled-frame {
  /* zoom: 0.5; */
  /* width: 350%;
  height: 100vh; */
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
    /* zoom: 0.5; */
    -moz-transform: scale(0.5);
    -o-transform: scale(0.5);
    -webkit-transform: scale(0.5);

  }
}
</style>