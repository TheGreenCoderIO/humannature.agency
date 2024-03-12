<script setup lang="ts">
  import logo from "@/assets/logo.svg";
  const sidebar = false
  const menuItems = [
        { title: 'About Us', path: '/' },
        { title: 'Projects', path: '/' },
        { title: 'Get In Touch', path: '/' }
   ]
</script>

<template>
      <v-app-bar color="black" dense fixed scroll-off-screen>
      <v-toolbar-title class="ml-15">
          <img :src="logo" />
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-xs-only mr-15">
        <v-btn
          flat
          class="no-uppercase"
          v-for="item in menuItems"
          :key="item.title">
          {{ item.title }}
        </v-btn>
      </v-toolbar-items>
    </v-app-bar>
</template>

<style scoped>
.navbar {
  color: #EAEAEA;
}
.no-uppercase {
    text-transform: unset !important;
}
</style>
