<script setup lang="ts">
import { ref } from 'vue';
import { useRouter } from 'vue-router';
import logo from "@/assets/logo.svg";

const drawer = ref(false);
const router = useRouter();

const menuItems = [
  { title: 'Home', path: '/' },
  { title: 'About', path: '/about' },
];

const openMail = () => {
  window.location.href = 'mailto:info@humannature.agency';
};
</script>

<template>
  <v-app-bar color="black gutter" class="mb-4 pt-4 ">
    <v-app-bar-nav-icon @click="drawer = !drawer" class="hidden-md-and-up">
    </v-app-bar-nav-icon>
    <v-toolbar-title class="ml-0">
      <v-btn @click="router.push('/')" class="width"><img :src="logo" class="logo" /></v-btn>
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items class="hidden-sm-and-down nav-text">
      <v-btn
        v-for="item in menuItems"
        :key="item.title"
        flat
        @click="router.push(item.path)"
      >
        {{ item.title }}
      </v-btn>
      <v-btn class="nav-btn" @click="openMail">
        Get In Touch
      </v-btn>
    </v-toolbar-items>
  </v-app-bar>

  <v-navigation-drawer
    v-model="drawer"
    app
    temporary
    class="hidden-md-and-up"
  >
    <v-list>
      <v-list-item v-for="item in menuItems" :key="item.title">
        <v-list-item-title @click="router.push(item.path)">{{ item.title }}</v-list-item-title>
      </v-list-item>
      <v-list-item>
        <v-btn class="nav-btn" @click="openMail">
          Get In Touch
        </v-btn>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
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
  font-family: 'Urbanist', sans-serif !important;
}

.logo {
  max-height: 20px;
}

@media (max-width: 932px) {
   .width{
    width: 10em;
    height: 5em;
   }
   .logo {
     width: 100px;
   }
}
</style>
