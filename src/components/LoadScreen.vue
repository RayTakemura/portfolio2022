<template>
  <div class="h-screen my-auto">
    <!-- <svg class="animate-spin h-5 w-5 mr-3" viewBox="0 0 24 24">
      <img :src="require(`@/assets/logo.png`)" alt="" />
    </svg>
    Processing...
    <img :src="require(`@/assets/logo.png`)" alt="" /> -->
    <div class="h-2/5"></div>
    <svg version="1.1" id="L3" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px"
      y="0px" viewBox="0 0 100 100" enable-background="new 0 0 0 0" xml:space="preserve">
      <circle fill="none" stroke="#FFB500" stroke-width="4" cx="50" cy="50" r="44" style="" />
      <circle fill="#6CCCC8" stroke="#6CCCC8" stroke-width="3" cx="8" cy="54" r="6">
        <animateTransform attributeName="transform" dur="2s" type="rotate" from="0 50 48" to="360 50 52"
          repeatCount="indefinite" />

      </circle>
    </svg>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
svg {
  width: 100px;
  height: 100px;
  margin: auto;
  display: block;
}
</style>