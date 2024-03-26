<script setup lang="ts">
</script>

<template>
  <v-container fluid class="landing mt-10 mb-10 justify-center align-center" >
    <v-row no-gutters>
       <v-col cols="12" sm="12" md="6" class="mx-auto mt-10 mb-10">
        <h1 class="wide">Building <span class="green">better brands</span> for
          a <span class="green">better planet.</span></h1>
        <h2>Storytelling & brand building for purpose-driven brands impacting sustainability, equality, and education.</h2>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
h1 {
  font-size: 5em;
}
h2 {
  font-size: 1.5em;
}
.landing {
  width: 100%;
  padding: 0;
  margin: 0;
  color: white;
  background-image: url('@/assets/background-one.png');
  background-size: contain;
}
@media (max-width: 1024px) {
  h1 {
    font-size: 3em;
  }
  h2 {
    font-size: 0.5em;
  }
}
</style>
