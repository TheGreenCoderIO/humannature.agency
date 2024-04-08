<script setup lang="ts">
</script>

<template>
  <v-container fluid class="landing mt-10 mb-10 justify-center text-center align-center" >
    <v-row no-gutters>
       <v-col cols="12" sm="12" md="12" class="pl-15 pr-15 pt-15 pb-15 mt-15 mb-15">
        <h1 class="wide">Building <span class="green">better brands</span> for
          a <span class="green">better planet.</span></h1>
        <h2>Storytelling & brand building for purpose-driven brands impacting sustainability, equality, and education.</h2>
      </v-col>
    </v-row>
  </v-container>
  <v-container fluid class="para">
    <v-row no-gutters>
      <v-col cols="12" sm="12" md="12" class="mx-auto pl-15 pr-15 mt-10 mb-10">
        <p class="para">Whether you’re part of an <strong>enterprise</strong> looking to
        develop a <strong>more sustainable UX </strong> or a 
        <strong>start-up</strong> with a dream to make education more
        accessible, we work with you to define and deliver the core of your
        brand, project or goal.</p> 

        <p class="para">Through <strong>storytelling</strong> and <strong>brand development</strong>, we help you echo that
        core for employees, stakeholders and customers to buy into.</p>
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
}

@media (max-width: 1024px) {
  h1 {
    font-size: 3em;
  }
  h2 {
    font-size: 1em;
  }
}
</style>
