<template>
  <v-app :dark="false">
    <v-app-bar fixed app>
      <v-app-bar-nav-icon>
        <v-icon>mdi-triangle-outline</v-icon>
      </v-app-bar-nav-icon>
      <v-toolbar-title>Daskemm</v-toolbar-title>
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>
