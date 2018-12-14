<template>
  <v-toolbar
    class="info"
    app
    fixed
    :clipped-left="true"
  >
    <v-toolbar-side-icon @click="$root.$emit('openLeftDrawer')" />
    <v-toolbar-title><img src="~/assets/images/logo.png" height="60"></v-toolbar-title>
    <v-spacer></v-spacer>
    <v-btn icon href="/" nuxt>
      <v-icon>home</v-icon>
    </v-btn>
    <v-btn icon href="/" nuxt>
      <v-icon>info</v-icon>
    </v-btn>
  </v-toolbar>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      title: 'PBDesk',
    };
  },
};
</script>

<style scoped>

</style>
