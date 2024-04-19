<script setup lang="ts">
  import logo from "@/assets/logo.svg";
  const sidebar = false
  const menuItems = [
        { title: 'Home', path: '/' },
        { title: 'About', path: '/about' },
   ]
  const openMail = () => {
    window.location.href = 'mailto:info@humannature.agency';
  };
</script>

<template>
      <v-app-bar color="black" class="mb-4 pt-4">
      <v-toolbar-title class="ml-15">
          <img :src="logo" class="logo"/>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-xs-only mr-15 nav-text" align="center" justify="center">
        <v-btn
          @click="$router.push(item.path)"
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

.nav-text {
  font-family: 'Urbanist', san-serif !important;
}

.logo {
  max-height: 20px;
}
</style>
