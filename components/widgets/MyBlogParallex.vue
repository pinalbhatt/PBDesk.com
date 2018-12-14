<template>
  <v-parallax
    dark
    :src="require('@/assets/images/homebg.jpg')"
  >
    <v-layout
      align-center
      column
      justify-center
    >
      <h4 class="subheading">Visit My Blog!</h4>
      <h1 class="display-2 font-weight-thin mb-3">Pinal Bhatt's Blog</h1>
      <h1 class="display-2 font-weight-thin mb-3">Learning Endeavor Forever...</h1>
      <v-btn color="info">Info</v-btn>
    </v-layout>
  </v-parallax>
</template>

<script>
export default {
  name: 'MyBlogParallex',
};
</script>

<style scoped>

</style>
