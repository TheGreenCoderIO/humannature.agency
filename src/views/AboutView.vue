<script setup lang="ts">
import NavBar from '../components/NavBar.vue'
import Footer from '../components/Footer.vue'
import AboutBody from '../components/AboutBody.vue'
import Goals from '../components/Goals.vue'
import ChangeMakers from '../components/ChangeMakers.vue'
</script>

<template>
  <NavBar />
  <v-main app class="main gutter">
    <ChangeMakers />
    <AboutBody />
    <Goals />
    <Footer />
  </v-main>
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

@media (max-width: 1024px) {
  .gutter {
    padding-left: 0% !important;
    padding-right: 0% !important;
  }

}
</style>
