<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
    <v-app-bar-nav-icon/>

    <v-toolbar-title>Hello, World</v-toolbar-title>

    <v-spacer></v-spacer>

    <v-btn icon>
      <v-icon>mdi-magnify</v-icon>
    </v-btn>

    </v-app-bar>

    <v-content app>
      <router-view/>
    </v-content>
    <v-footer color="primary" dark>
      <v-spacer/>Copyright twk1024 2021
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'App',
};
</script>
