<template>
  <div class="grid grid-cols-1 lg:grid-cols-2 h-screen ">
    <div class="grid grid-cols-1 justify-center lg:content-center mt-auto lg:mt-0 lg:mr-14">
      <div class="text-4xl  xl:text-6xl lg:text-right text-white">
        Hi 👋🏼
      </div>
      <div class="text-4xl  xl:text-6xl lg:text-right text-white ">
        <span>I'm </span>
        <span class="font-extrabold bg-clip-text text-transparent bg-gradient-to-r from-teal-500 to-orange-500">Ray
          Takemura</span>
      </div>
    </div>
    <div class="container m-auto lg:ml-14" id="wrap">
      <iframe class="responsive-iframe" id="scaled-frame"
        src='https://my.spline.design/untitled-e0a1d03472edbe77f3631bf8d12c4d28/' frameborder='0'></iframe>

    </div>

  </div>


</template>

<script>
export default {

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
    zoom: 1;
    -moz-transform: scale(0.3);
    -o-transform: scale(0.3);
    -webkit-transform: scale(0.3);

  }
}
</style>