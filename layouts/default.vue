<template>
  <v-app>
    <!--<v-navigation-drawer-->
      <!--:mini-variant="false"-->
      <!--:clipped="clipped"-->
      <!--v-model="drawer"-->
      <!--fixed-->
      <!--temporary-->
    <!--&gt;-->
      <!--<v-list>-->
        <!--<v-list-tile-->
          <!--v-for="(item, i) in items"-->
          <!--:to="item.to"-->
          <!--:key="i"-->
          <!--router-->
          <!--exact-->
        <!--&gt;-->
          <!--<v-list-tile-action>-->
            <!--<v-icon v-html="item.icon" />-->
          <!--</v-list-tile-action>-->
          <!--<v-list-tile-content>-->
            <!--<v-list-tile-title v-text="item.title" />-->
          <!--</v-list-tile-content>-->
        <!--</v-list-tile>-->
      <!--</v-list>-->
    <!--</v-navigation-drawer>-->
    <Drawer></Drawer>
    <Header></Header>
    <!--<v-toolbar-->
      <!--:clipped-left="clipped" app-->
    <!--&gt;-->
      <!--<v-toolbar-side-icon @click="drawer = !drawer" />-->
      <!--<v-btn-->
        <!--icon-->
        <!--@click.stop="clipped = !clipped"-->
      <!--&gt;-->
        <!--<v-icon>web</v-icon>-->
      <!--</v-btn>-->
      <!--<v-btn-->
        <!--icon-->
        <!--@click.stop="fixed = !fixed"-->
      <!--&gt;-->
        <!--<v-icon>remove</v-icon>-->
      <!--</v-btn>-->
      <!--<v-toolbar-title v-text="title"/>-->
      <!--<v-btn-->
        <!--icon-->
        <!--@click.stop="rightDrawer = !rightDrawer"-->
      <!--&gt;-->
        <!--<v-icon>menu</v-icon>-->
      <!--</v-btn>-->
    <!--</v-toolbar>-->
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
    <Footer></Footer>
  </v-app>
</template>

<script>
import Header from '@/components/common/Header';
import Footer from '@/components/common/Footer';
import Drawer from '../components/common/Drawer';

export default {
  components: {
    Header,
    Footer,
    Drawer,
  },
  data() {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [
        { icon: 'apps', title: 'Welcome', to: '/' },
        { icon: 'bubble_chart', title: 'Inspire', to: '/inspire' },
      ],
      miniVariant: false,
      right: true,
      title: 'Vuetify.js',
    };
  },
};
</script>
