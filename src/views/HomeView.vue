<script setup lang="ts">
import NavBar from '../components/NavBar.vue'
import Footer from '../components/Footer.vue'
import HomeLanding from '../components/HomeLanding.vue'
</script>

<template>
  <NavBar />
  <v-main app class="main">
    <HomeLanding />
  </v-main>
  <Footer />
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

.main {
  background-color: #000;
}
</style>
