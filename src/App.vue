<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
    <v-app-bar-nav-icon @click="drawer = !drawer"/>

    <sendTitle :title="title"/>
    <v-spacer></v-spacer>

    <v-btn icon>
      <v-icon>mdi-magnify</v-icon>
    </v-btn>

    </v-app-bar>
    
    <v-navigation-drawer app v-model="drawer">
      <navMenu :navtitle="navtitle" :subtitle="subtitle"/>
    </v-navigation-drawer>

      <v-divider></v-divider>
    
    <v-content app>
      <router-view/>
    </v-content>
    <sendFooter :footer="footer"/>
  </v-app>
</template>

<script>
import sendTitle from '@/components/title'
import navMenu from '@/components/menu'
import sendFooter from '@/components/footer'

export default {
  name: 'App',
  components: {sendTitle, navMenu ,sendFooter},
  data () {
    return {
      drawer: false,
      title: "Hello, World",
      footer: "© 2021 Taewon Kim (dokidia)",
      navtitle: "Main Menu",
      subtitle: "Subtitle"
    }
  }
}
</script>
