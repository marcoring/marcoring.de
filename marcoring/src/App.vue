<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    > 
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <div id="app">
        <v-app id="inspire">
          <v-toolbar dark absolute class="homepage-toolbar">
          <v-toolbar-side-icon></v-toolbar-side-icon>
          <v-toolbar-title>Title</v-toolbar-title>
          <v-spacer></v-spacer>
          <v-toolbar-items class="hidden-sm-and-down">
        </v-toolbar-items>
       </v-toolbar>
    
        <section style="height: 100vh;">
          <v-parallax 
            dark 
            src="https://townshipcanada.com/static/pattern.svg">
            <!--:src="require('@/assets/pic1.jpg')"-->
            <v-layout white--text align-center column justify-center style="margin-top: 8.5em;">
              <h3 class=" display-3 ma-2 text-xs-center">Vuetify.js</h3>
              <h4 class="subheading">Build your application today!</h4>
              <v-flex row wrap text-xs-center>
              <v-btn dark large color="blue lighten-2" class="mt-4 elevation-0">login</v-btn>
              <v-btn dark large color="blue lighten-2" class="mt-4 elevation-0">signup</v-btn>
              </v-flex>
            </v-layout>
          </v-parallax>
        </section>
        </v-app>
      </div>
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>

<style scoped>

  .homepage-toolbar {
    background: rgba(222,222,222,0.4) !important;
    background: transparent !important;
    -webkit-box-shadow: none !important;
    box-shadow: none !important;
  }

</style>
