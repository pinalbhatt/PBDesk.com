<template>
  <v-app>
    <Drawer></Drawer>
    <Header></Header>
    <v-content>
      <section style="margin-bottom: 0">
        <banner></banner>
      </section>
      <nuxt />
    </v-content>
    <Footer></Footer>
  </v-app>
</template>

<script>
import Header from '@/components/common/Header';
import Footer from '@/components/common/Footer';
import Drawer from '../components/common/Drawer';
import Banner from '../components/home/Banner';

export default {
  components: {
    Header,
    Footer,
    Drawer,
    Banner,
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
