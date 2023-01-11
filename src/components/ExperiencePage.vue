<template>
  <div class=" grid grid-cols-1 lg:grid-cols-2 lg:mr-40">
    <div class="mt-20 title-text-size2 ">
      <span class="my-20 bold-theme-text mr-2">Experience</span><span>💼</span>
    </div>
    <div class="lg:hide"></div>
  </div>
  <div class="grid grid-cols-1 ">
    <template v-for="card, i in expCardArr" :key="`card${i}`">
      <div :class="`flex justify-center mx-12 ${i === 0 ? 'mt-10' : 'mt-20'} xl:mx-10`">
        <div class="border-2 rounded-sm border-slate-500  w-fit flex justify-center flex-col max-w-lg">
          <div :class="`${card?.imgBackGroundColor} ${card?.imgBorder} m-5 lg:m-8 lg:mb-6 mb-2`">
            <img :src="require(`@/assets/${card?.img}`)" :alt="card?.imgAlt" width="500" height="100%">
          </div>
          <div class="font-bold mb-2 lg:mb-6 flex flex-col justify-center "><span class="lg:mr-2">{{
    card.company
}}</span><span>({{ card.title }})</span></div>
          <div class="border border-slate-500 mx-10 mb-2 lg:mb-6" />
          <ul class="list-disc  text-left ml-8 mr-2 mb-2 lg:mb-6 ">
            <template v-for="point, i in card.details" :key="`detail${i}`">
              <li>{{ point }}</li>
            </template>
          </ul>
        </div>

      </div>
    </template>
  </div>
</template>

<script>
export default {
  data() {
    return {
      expCardArr: [
        {
          img: 'fexlogo.png',
          imgAlt: "Fulfillment Express logo",
          imgBackGroundColor: 'bg-white',
          imgBorder: 'border-2 rounded border-amber-900',
          company: "Fulfillment Express INC. / OpCenter LLC",
          title: "Full Stack Web Developer",
          details: [
            "Build RESTful API with Laravel and Eloquent (ORM) to reliably access and use data from the database",
            "Implement and customize front-end components using Vue.js while utilizing SCSS and frontend toolkits such as Bootstrap and PrimeVue",
            "Design project mock-ups using interface design tools, such as Figma and Draw.io",
            "Launch the staging and development environment by merging branches with Git and GitHub",
            "Coach new developers to follow existing coding conventions and debug code",
          ],
        },
      ]
    }
  },
  computed: {
  }
}
</script>

<style  scoped>

</style>