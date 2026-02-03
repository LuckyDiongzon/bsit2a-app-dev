<template>
  <v-app>
  <v-app-bar :elevation="2">
  <template v-slot:prepend>
    <v-app-bar-nav-icon @click="drawer = !drawer; rail = !rail"></v-app-bar-nav-icon>
  </template>

  <v-app-bar-title>Application Bar</v-app-bar-title>
</v-app-bar>

    <v-navigation-drawer v-model=" drawer" 
    :rail="rail"
    permanent>
      
        <template v-slot:prepend>
          <v-list-item
            lines="two"
            prepend-avatar=c:\Users\SNCBT\Documents\607158395_1876656183221085_2326868583434191434_n.jpg
            subtitle="Logged in"
            title="Adrian Diongzon"
          ></v-list-item>
        </template>

        <v-divider></v-divider>

        <v-list density="compact" nav>
          <v-list-item prepend-icon="mdi-home-city" title="Home" value="home"></v-list-item>
          <v-list-item prepend-icon="mdi-account" title="My Account" value="account"></v-list-item>
          <v-list-item prepend-icon="mdi-account-group-outline" title="Users" value="users"></v-list-item>
        </v-list>
      </v-navigation-drawer>
    <v-main>
      <v-container fluid>
        <slot />
      </v-container>
    </v-main>

  </v-app>
</template>

<script setup>
import { ref } from 'vue'
const drawer = ref(true);
const rail = ref(true)

</script>

<style>

</style>