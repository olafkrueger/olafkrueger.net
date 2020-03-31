<template>
   <v-app light>

    <v-app-bar app dense color='white' flat>
      olafkrueger.net
      <v-spacer />
      Contact
    </v-app-bar>
    
      <v-content>
          <v-img
            :min-height="'calc(100vh - ' + $vuetify.application.top + 'px)'"
            src="./assets/me3.jpg"
          >          
        <v-divider />
          <v-container fill-height>
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
                      class="display-4 font-weight-thin white--text pa-3"
                    >
                      driven by passion
                    </v-row>
                    <v-row
                      align="center"
                      justify="center"
                      class=" pa-3"
                    >
                      <div class="pa-1" v-for="(tag, i) in tags"
                          :key="i">
                        <v-chip
                          outlined
                          :color="tag.color"
                          :key="tag.id"
                          >
                          {{tag.text}}
                        </v-chip>
                      </div>                 
                    </v-row>                  
                  </v-container>
                </v-card>
              </v-col>
          
            </v-row>
            <v-row    
              align="center"
              justify="center"
              class=" pa-3"
            >
            
              <v-col cols="12" xs="12" sm="12" md="12">
                <v-card>
                  <v-card-title>About me</v-card-title>
                  <v-card-text>Vuejs, NodeJS, Fastify, JAMStack, REST, SAP, ABAP, Apache Flex, Apache Royale, AS3, PHP</v-card-text>
                </v-card>
              </v-col>
            
            
              <!--
              <v-col cols="12" xs="12" sm="12" md="4">
                <v-card>
                  <v-card-title>Open</v-card-title>
                  <v-card-text></v-card-text>
                </v-card>
              </v-col>
              <v-col cols="12" xs="12" sm="12" md="4">
                <v-card>
                  <v-card-title>Neuguerig</v-card-title>
                </v-card> 
              </v-col>   
              -->      
      <!--
      <section id="about-me">
        <div class="py-12"></div>

        <v-container class="text-center">
          <h2 class="display-2 font-weight-bold white--text mb-3">ABOUT ME</h2>

          <v-responsive
            class="mx-auto mb-8"
            width="56"
          >
            <v-divider class="mb-1"></v-divider>

            <v-divider></v-divider>
          </v-responsive>

          <v-responsive
            class="mx-auto title font-weight-light white--text mb-8"
            max-width="720"
          >
            Vuetify is the #1 component library for Vue.js and has been in active development since 2016. The goal of the project is to provide users with everything that is needed to build rich and engaging web applications using the Material Design specification. It accomplishes that with a consistent update cycle, Long-term Support (LTS) for previous versions, responsive community engagement, a vast ecosystem of resources and a dedication to quality components.
          </v-responsive>

          <v-avatar
            class="elevation-12 mb-12"
            size="128"
          >
            <v-img src="https://cdn.vuetifyjs.com/images/john.png"></v-img>
          </v-avatar>

          <div></div>

          <v-btn
            color="grey"
            href="https://vuetifyjs.com"
            outlined
            large
          >
            <span class="grey--text text--darken-1 font-weight-bold">
              Vuetify Documentation
            </span>
          </v-btn>
        </v-container>

        <div class="py-12"></div>
      </section> 
      -->                     
            </v-row>
            
          </v-container>
          
          </v-img>
        </v-content>
    <!--
    <v-carousel v-model="model">
      <v-carousel-item
        v-for="(view) in views"
        :key="view.color"
      >
        <v-sheet
          :color="view.color"
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
                      {{view.title}}
                    </v-row>
                    <v-row
                      align="center"
                      justify="center"
                      class=" pa-3"
                    >
                      <div class="pa-1" v-for="(tag, i) in view.tags"
                          :key="i">
                        <v-chip
                          outlined
                          color="white"
                          :key="tag.id"
                          >
                          {{tag.text}}
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
    -->
    <!--
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
                      <div class="headline text-center">Passionized</div>
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
                      <div class="headline text-center">Open</div>
                    </v-card-title>
                    <v-card-text>
                      Always question the status quo!

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
      -->
  </v-app>
</template>

<script>

export default {
  name: 'App',

  components: {

  },

  data: () => ({
    tags: [
      { text:'Father', icon:'' , color: 'white'},
     // { text:'Husband', icon:'', color: 'grey' },
      { text:'Developer', icon:'', color: 'white' },
    //{ text:'Enthusiast', icon:'', color: 'grey' },
      { text:'Fool', icon:'', color: 'white' },

    ],
    views: [
      {
        title: 'driven by passion',
        color: 'red',
        tags: [
          { text:'Vuejs', icon:'' },
          { text:'NodeJS', icon:'' },
          { text:'SAP', icon:'' },
        ]
      },
      {
        title: 'work',
        color: 'primary',
        tags: [
          { text:'Vuejs', icon:'' },
          { text:'NodeJS', icon:'' },
          { text:'SAP', icon:'' },
        ]
      },
      {
        title: 'life',
        color: 'orange',
        tags: [
          { text:'Vuejs', icon:'' },
          { text:'NodeJS', icon:'' },
          { text:'SAP', icon:'' },
        ]
      },
      {
        title: 'contact',
        color: 'yellow darken-2',
        tags: [
          { text:'mail@olafkrueger.net', icon:'' },
          { text:'GitHub', icon:'' },
          { text:'Twitter', icon:'' },
          { text:'LinkedIn', icon:'' },
          { text:'Xing', icon:'' },
        ]
      },
    ],
    title: "",
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
