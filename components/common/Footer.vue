<template>
  <div>
    <section>
      <ad-responsive></ad-responsive>
    </section>
    <v-footer class="blue darken-2" :clipped-left="true" :fixed="false">
      <v-layout row wrap align-center>
        <v-flex xs12>
          <div class="white--text ml-3 text-md-center">
            With
            <v-icon class="red--text">favorite</v-icon>
            from the desk of <a class="white--text" href="/">Pinal Bhatt</a>.
          </div>
        </v-flex>
      </v-layout>
  </v-footer>
  </div>
</template>

<script>
import AdResponsive from '../ad/ResponsiveAd';

export default {
  name: 'Footer',
  components: {
    AdResponsive,
  },
};
</script>

<style scoped>

</style>
