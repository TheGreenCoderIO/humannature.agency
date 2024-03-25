<script setup lang="ts">
  import logo from "@/assets/logo.svg";
  const sidebar = false
  const menuItems = [
        { title: 'Home', path: '/' },
        { title: 'About', path: '/' },
   ]
  const openMail = (mailto) => {
    window.location.href = 'mailto:info@humannature.agency';
  };
</script>

<template>
      <v-app-bar color="black" fixed scroll-off-screen class="mt-4 mb-4">
      <v-toolbar-title class="ml-15">
          <img :src="logo" class="logo"/>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-xs-only mr-15" align="center" justify="center">
        <v-btn
          flat
          v-for="item in menuItems"
          :key="item.title">
          {{ item.title }}
        </v-btn>
        <v-btn class="nav-btn" @click="openMail">
          Get In Touch
        </v-btn>
      </v-toolbar-items>
    </v-app-bar>
</template>

<style scoped>
.navbar {
  color: #EAEAEA;
  max-height: 20px;
}
.nav-btn {
  background-color: #09C771;
  color: #000;
}

.logo {
  max-height: 20px;
}
</style>
