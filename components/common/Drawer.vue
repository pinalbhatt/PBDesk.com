<template>
  <v-navigation-drawer
    :mini-variant="false"
    :clipped="false"
    v-model="drawer"
    fixed
    temporary
  >
    <v-list>
      <v-list-tile
        v-for="(item, i) in items"
        :to="item.to"
        :key="i"
        router
        exact
      >
        <v-list-tile-action>
          <v-icon v-html="item.icon" />
        </v-list-tile-action>
        <v-list-tile-content>
          <v-list-tile-title v-text="item.title" />
        </v-list-tile-content>
      </v-list-tile>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
export default {
  name: 'Drawer',
  data() {
    return {
      drawer: false,
      items: [
        { icon: 'apps', title: 'Welcome', to: '/' },
        { icon: 'bubble_chart', title: 'Inspire', to: '/inspire' },
      ],
    };
  },
  methods: {
    toggleDrawer() {
      this.drawer = !this.drawer;
    },
  },
  created() {
    this.$root.$on('openLeftDrawer', this.toggleDrawer);
  },
};
</script>

<style scoped>

</style>
