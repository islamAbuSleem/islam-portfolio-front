<script setup>
import { ref } from 'vue'
const drawer = ref(true)
const rail = ref(true)
</script>

<template>
  <nav>
    <v-navigation-drawer class="bg-primary" v-model="drawer" :rail="rail" permanent>
      <v-list-item prepend-avatar="https://randomuser.me/api/portraits/men/85.jpg" title="Islam Abu sleem" nav>
      </v-list-item>

      <v-divider></v-divider>

      <v-list density="compact" nav>
        <v-list-item prepend-icon="mdi-home-city" title="Overview" value="Overview"></v-list-item>
        <v-list-item prepend-icon="mdi-account" title="Experience" value="account"></v-list-item>
        <v-list-item prepend-icon="mdi-account-group-outline" title="Projects" value="Projects"></v-list-item>
        <v-list-item prepend-icon="mdi-account-group-outline" title="Skills" value="Skills"></v-list-item>
        <v-list-item prepend-icon="mdi-account-group-outline" title="Contacts" value="Contacts"></v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar app clipped flat>
      <template v-slot:prepend>
        <v-app-bar-nav-icon @click="rail = !rail"></v-app-bar-nav-icon>
      </template>
      <v-toolbar-title class="grey--text">
        <span class="font-weight-thin text-capitalize text-secondary">Islam</span>
        <span class="text-capitalize text-secondary">Abusleem</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-behance</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-github</v-icon>
      </v-btn>

      <v-btn icon class="mr-5">
        <v-icon>mdi-linkedin</v-icon>
      </v-btn>
    </v-app-bar>

  </nav>
</template>
