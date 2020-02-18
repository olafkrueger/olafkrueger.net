<template>
   <v-app light>

    <v-content>
            <v-toolbar color="transparent" dense dark>
      <v-toolbar-title v-text="title"></v-toolbar-title>
    </v-toolbar>
    <v-carousel v-model="model">
      <v-carousel-item
        v-for="(color) in colors"
        :key="color"
      >
        <v-sheet
          :color="color"
          height="100%"
          tile
        >
          <v-container class="fill-height">
            <v-row
              align="center"
              justify="center"
            >
              <v-col cols="12">
                <v-card flat color="transparent">
                  <v-container>
                    <v-row
                      align="center"
                      justify="center"
                      class="display-4 font-weight-thin pa-3"
                    >
                      driven by passion
                    </v-row>
                    <v-row
                      align="center"
                      justify="center"
                      class=" pa-3"
                    >
                      <div class="pa-1" v-for="(item, i) in items"
                          :key="i">
                        <v-chip
                          outlined
                          color="white"
                          :key="item.id"
                          >
                          {{item.text}}
                        </v-chip>
                      </div>
                      <div class="pa-1">
                        <v-chip 
                          outlined
                          color="white"
                          >
                          NodeJS
                        </v-chip>
                      </div>                  
                    </v-row>                  
                  </v-container>
                </v-card>
              </v-col>
            </v-row>
          </v-container>  
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
      <section>
        <v-layout
          column
          wrap
          class="my-12"
          align-center
        >
          <v-flex xs12 sm4 class="my-4">
            <div class="text-center">
              <h2 class="headline">The best way to start developing</h2>
              <span class="subheading">
                Cras facilisis mi vitae nunc
              </span>
            </div>
          </v-flex>
          <v-flex xs12>
            <v-container grid-list-xl>
              <v-layout row wrap align-center>
                <v-flex xs12 md4>
                  <v-card flat class="transparent">
                    <v-card-text class="text-center">
                      <v-icon x-large class="blue--text text--lighten-2">mdi-palette</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-center">Material Design</div>
                    </v-card-title>
                    <v-card-text>
                      Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare.
                      Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.
                      Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti.
                    </v-card-text>
                  </v-card>
                </v-flex>
                <v-flex xs12 md4>
                  <v-card flat class="transparent">
                    <v-card-text class="text-center">
                      <v-icon x-large class="blue--text text--lighten-2">mdi-flash</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline">Fast development</div>
                    </v-card-title>
                    <v-card-text>
                      Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare.
                      Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.
                      Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti.
                    </v-card-text>
                  </v-card>
                </v-flex>
                <v-flex xs12 md4>
                  <v-card flat class="transparent">
                    <v-card-text class="text-center">
                      <v-icon x-large class="blue--text text--lighten-2">mdi-wrench</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-center">Completely Open Sourced</div>
                    </v-card-title>
                    <v-card-text>
                      Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare.
                      Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.
                      Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti.
                    </v-card-text>
                  </v-card>
                </v-flex>
              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
      </section>

      <section>
        <v-parallax src="assets/section.jpg" height="380">
          <v-layout column align-center justify-center>
            <div class="headline white--text mb-4 text-center">Web development has never been easier</div>
            <em>Kick-start your application today</em>
            <v-btn
              class="mt-12"
              color="blue lighten-2"
              dark
              large
              href="/pre-made-themes"
            >
              Get Started
            </v-btn>
          </v-layout>
        </v-parallax>
      </section>

      <section>
        <v-container grid-list-xl>
          <v-layout row wrap justify-center class="my-12">
            <v-flex xs12 sm4>
              <v-card flat class="transparent">
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline">Company info</div>
                </v-card-title>
                <v-card-text>
                  Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare.
                  Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.
                  Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti.
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 sm4 offset-sm1>
              <v-card flat class="transparent">
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline">Contact us</div>
                </v-card-title>
                <v-card-text>
                  Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare.
                </v-card-text>
                <v-list class="transparent">
                  <v-list-item>
                    <v-list-item-action>
                      <v-icon class="blue--text text--lighten-2">mdi-phone</v-icon>
                    </v-list-item-action>
                    <v-list-item-content>
                      <v-list-item-title>777-867-5309</v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-action>
                      <v-icon class="blue--text text--lighten-2">mdi-map-marker</v-icon>
                    </v-list-item-action>
                    <v-list-item-content>
                      <v-list-item-title>Chicago, US</v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-action>
                      <v-icon class="blue--text text--lighten-2">mdi-email</v-icon>
                    </v-list-item-action>
                    <v-list-item-content>
                      <v-list-item-title>john@vuetifyjs.com</v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                </v-list>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>
      </section>

      <v-footer color="blue darken-2">
        <v-layout row wrap align-center>
          <v-flex xs12>
            <div class="white--text ml-4">
              Made with
              <v-icon class="red--text">mdi-heart</v-icon>
              by <a class="white--text" href="https://vuetifyjs.com" target="_blank">Vuetify</a>
              and <a class="white--text" href="https://github.com/vwxyzjn">Costa Huang</a>
            </div>
          </v-flex>
        </v-layout>
      </v-footer>
    </v-content>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  components: {

  },

  data: () => ({
    items: [
      { text:'Vuejs', icon:'' },
      { text:'NodeJS', icon:'' },
      { text:'SAP', icon:'' },
    ],
    title: "olafkrueger.net",
        colors: [
          'primary',
          'secondary',
          'yellow darken-2',
          'red',
          'orange',
        ],
        model: 0,  
  }),
};
</script>
