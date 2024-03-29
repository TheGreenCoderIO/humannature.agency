<script setup lang="ts">
</script>

<template>
  <v-container fluid class="landing mt-10 mb-10 justify-center align-center" >
    <v-row no-gutters>
       <v-col cols="12" sm="12" md="6" class="mx-auto mt-10 mb-10">
        <h1 class="wide">
            We work with the
            <span class="green">change-makers.</span>
        </h1>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
h1 {
  font-size: 5em;
  line-height: 1em;
  padding-bottom:20px;
}
h2 {
  font-size: 1.5em;
  font-weight: bold;
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
