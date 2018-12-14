<template>
  <div>
    <section>
      <v-layout
        column
        wrap
        class="mt-5"
        align-center
      >
        <v-flex xs12 sm4 class="my-3">
          <div class="text-xs-center">
            <h2 class="headline">Welcome to my Desk!</h2>
            <!--<span class="subheading">-->
                <!--Cras facilisis mi vitae nunc-->
              <!--</span>-->
          </div>
        </v-flex>
        <v-flex xs12>
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex xs12 md6>
                <v-card class="elevation-0 transparent">
                  <v-card-text class="text-xs-justify subheading">
                    Hi Everyone! I’m <b>Pinal Bhatt</b> and I am a <em>Software Engineer</em>, so yes always on learning ramp!
                    On this site you’ll find interesting posts, articles, tutorials, videos, news updates and links on Programming,
                    Microservices, Cloud & Serverless, JavaScript, NodeJS, TypeScript, Vue, Angular, React, GoLang
                    and other random thoughts and opinions.
                    And ofcourse my tips for healthy eating and leaving! After all <b>Health Is Wealth !!! :)</b>”
                  </v-card-text>
                </v-card>
              </v-flex>
              <v-flex xs12 md6>
                <v-card class="elevation-0 transparent">
                  <v-card-text class="text-xs-justify subheading">
                    I created this site to share my coding and technology learning experiences.
                    I am a self learner and I like sharing my experiments, ideas and experience with everyone by
                    writing articles on latest technology and trends. I feel pleased and pride by sharing my knowledge
                    and information that I have gained over time. And this site is my heartily attempt towards this.
                    I believe in sharing and I am a strong supporter of Open-Source as well.
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
        <!--<v-flex xs12 sm4 class="my-3">-->
          <!---->
        <!--</v-flex>-->
      </v-layout>
    </section>
    <section>
      <my-blog-parallex></my-blog-parallex>
    </section>
    <v-layout
      column
      justify-center
      align-center>
      <v-flex
        xs12
        sm8
        md6>
        <div class="text-xs-center">
          <logo/>
          <vuetify-logo/>
          <img src="~/assets/images/logo.png">
        </div>
        <v-card>
          <v-card-title class="headline">Welcome to the Vuetify + Nuxt.js template</v-card-title>
          <v-card-text>
            <p>Vuetify is a progressive Material Design component framework for Vue.js. It was designed to empower developers to create amazing applications.</p>
            <p>For more information on Vuetify, check out the <a
              href="https://vuetifyjs.com"
              target="_blank">documentation</a>.</p>
            <p>If you have questions, please join the official <a
              href="https://chat.vuetifyjs.com/"
              target="_blank"
              title="chat">discord</a>.</p>
            <p>Find a bug? Report it on the github <a
              href="https://github.com/vuetifyjs/vuetify/issues"
              target="_blank"
              title="contribute">issue board</a>.</p>
            <p>Thank you for developing with Vuetify and I look forward to bringing more exciting features in the future.</p>
            <div class="text-xs-right">
              <em><small>&mdash; John Leider</small></em>
            </div>
            <hr class="my-3">
            <a
              href="https://nuxtjs.org/"
              target="_blank">Nuxt Documentation</a>
            <br>
            <a
              href="https://github.com/nuxt/nuxt.js"
              target="_blank">Nuxt GitHub</a>
          </v-card-text>
          <v-card-actions>
            <v-spacer/>
            <v-btn
              color="primary"
              flat
              nuxt
              to="/inspire">Continue</v-btn>
          </v-card-actions>
        </v-card>
        <v-card>
          <v-card-title class="headline">Welcome to the Vuetify + Nuxt.js template</v-card-title>
          <v-card-text>
            <p>Vuetify is a progressive Material Design component framework for Vue.js. It was designed to empower developers to create amazing applications.</p>
            <p>For more information on Vuetify, check out the <a
              href="https://vuetifyjs.com"
              target="_blank">documentation</a>.</p>
            <p>If you have questions, please join the official <a
              href="https://chat.vuetifyjs.com/"
              target="_blank"
              title="chat">discord</a>.</p>
            <p>Find a bug? Report it on the github <a
              href="https://github.com/vuetifyjs/vuetify/issues"
              target="_blank"
              title="contribute">issue board</a>.</p>
            <p>Thank you for developing with Vuetify and I look forward to bringing more exciting features in the future.</p>
            <div class="text-xs-right">
              <em><small>&mdash; John Leider</small></em>
            </div>
            <hr class="my-3">
            <a
              href="https://nuxtjs.org/"
              target="_blank">Nuxt Documentation</a>
            <br>
            <a
              href="https://github.com/nuxt/nuxt.js"
              target="_blank">Nuxt GitHub</a>
          </v-card-text>
          <v-card-actions>
            <v-spacer/>
            <v-btn
              color="primary"
              flat
              nuxt
              to="/inspire">Continue</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
  </div>
</template>

<script>
import Banner from '../components/home/Banner';
import Logo from '~/components/Logo.vue';
import VuetifyLogo from '~/components/VuetifyLogo.vue';
import MyBlogParallex from '~/components/widgets/MyBlogParallex';

export default {
  layout: 'home',
  components: {
    Banner,
    Logo,
    VuetifyLogo,
    MyBlogParallex,
  },
  data() {
    return {
      aaa: '~/assets/images/homebg.jpg',
    };
  },
};
</script>
