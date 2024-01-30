<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <v-card
  elevation="3"
  max-width="1200"
  class="mx-auto"
  >
  <v-layout>
      <v-app-bar
       color="blue-darken-1"
       class="mb-100"
      >

      <template v-slot:prepend>
        <v-btn :to="{name: 'home'}">
          Inmobiliaria
        </v-btn>
      </template>
      
      <h2>Vuetify</h2>
      
      <template v-slot:append>

        <v-btn :to="{name:'home'}">
          Login
        </v-btn>

        <v-btn :to="{name:'login'}">
          Login
        </v-btn>
      </template>

      </v-app-bar>

        <v-main class="pt-30">
          <v-container>
            <RouterView/>
          </v-container>
        </v-main>

  </v-layout>

   
  </v-card>
</template>

