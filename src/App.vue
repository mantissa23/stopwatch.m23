<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>23.</span>
        <span class="font-weight-light">STOPWATCH</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        flat
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
      >
        <span class="mr-2">Latest Release</span>
      </v-btn>
    </v-toolbar>

    <v-content>
      <!-- <HelloWorld/> -->

       <v-container grid-list-md text-xs-center>
        <v-layout align-center justify-center row fill-height>
          <v-flex xs2>
            <v-card dark color="yellow">
              <v-card-text class="display-4 font-weight-bold">00</v-card-text>
            </v-card>
          </v-flex>

          <v-flex xs2>
            <v-card dark color="amber">
              <v-card-text class="display-4 font-weight-bold">00</v-card-text>
            </v-card>
          </v-flex>

          <v-flex xs2>
            <v-card dark color="orange">
              <v-card-text class="display-4 font-weight-bold">00</v-card-text>
            </v-card>
          </v-flex>
        </v-layout>
       </v-container>
    </v-content>

    <v-footer app class="pa-3">
      <v-spacer></v-spacer>
      <div class="caption">&copy; <a href="https://ma23.ru">Dmitriy Maziuk</a> {{ new Date().getFullYear() }}</div>
    </v-footer>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {},
  data: () => ({
    sec: 0,
    ms: 10,
  }),

  mounted () {
    // setInterval(() => {}, 10);
  },
}
</script>
