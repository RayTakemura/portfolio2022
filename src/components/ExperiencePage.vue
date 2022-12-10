<template>
  <!-- <div class="h-screen"> -->
  <div class=" grid grid-cols-1 lg:grid-cols-2 lg:mr-40">
    <div class="mt-20 title-text-size2 ">
      <span class="my-20 bold-theme-text mr-2">Experience</span><span>💼</span>
    </div>

    <div class="lg:hide"></div>
  </div>
  <!-- <img src="../assets/fexlogo.png" alt="test"> -->
  <div class="grid grid-cols-1 ">
    <template v-for="card, i in expCardArr" :key="`card${i}`">
      <!-- ${cardCol}  -->
      <div :class="`flex justify-center mx-20 mt-20 xl:mx-10`">
        <div class="border-2 shadow-inner rounded-lg shadow-white w-fit flex justify-center flex-col">
          <div :class="`${card?.imgBackGroundColor} ${card?.imgBorder} m-10`">
            <img :src="require(`@/assets/${card?.img}`)" :alt="card?.imgAlt" width="500" height="30%">
          </div>
          <div class="border border-slate-500 mx-10 mb-10" />
          <div>test</div>
        </div>

      </div>
      <!-- <div class="lg:col-span-12">
          123
        </div> -->
    </template>
  </div>
  <!-- </div> -->


</template>

<script>
// import fexlogo from "./../assets/fexlogo.png"
export default {
  data() {
    return {
      expCardArr: [
        {
          img: 'fexlogo.png',
          imgAlt: "Fulfillment Express logo",
          imgBackGroundColor: 'bg-white',
          imgBorder: 'border-2 rounded border-amber-900',
          title: null,
          details: null,
        },
        {
          img: 'fexlogo.png',
          imgAlt: "Fulfillment Express logo",
          imgBackGroundColor: 'bg-white',
          imgBorder: 'border-2 rounded border-amber-900',
          title: null,
          details: null,
        },
        // {
        //   img: 'fexlogo.png',
        //   imgAlt: "Fulfillment express logo",
        //   imgBackGroundColor: 'bg-white',
        //   imgBorder: 'border-2 rounded border-amber-900',
        //   title: null,
        //   details: null,
        // },
      ]
    }
  },
  computed: {
  }
}
</script>

<style lang="scss" scoped>

</style>