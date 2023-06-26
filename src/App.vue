<script setup>
import { useTheme } from 'vuetify'
import navbar from './components/navbar.vue'

const theme = useTheme()
function toggleTheme() {
  return theme.global.name.value = theme.global.current.value.dark ? 'light' : 'dark'
}

</script>

<template>
  <v-app>
    <v-layout>

      <navbar></navbar>
      <v-main class="main-content">
        <router-view></router-view>
      </v-main>
    </v-layout>
  </v-app>
</template>

<style scoped></style>
