<template>
  <v-parallax  :src="require('@/assets/images/homebg.jpg')" height="600" style="margin-bottom: -100px" >
    <v-layout
      column
      align-center
      justify-center
      class="white--text"
    >
      <img src="~/assets/images/logo.png" alt="Vuetify.js" height="200">
      <div class="subheading mb-3 text-xs-center">from the desk of</div>
      <h1 class="white--text mb-2 display-1 text-xs-center">Pinal Bhatt</h1>
    </v-layout>
  </v-parallax>
</template>

<script>
export default {
  name: 'Banner',
};
</script>

<style scoped>

</style>
