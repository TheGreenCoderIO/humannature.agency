<script setup lang="ts">

  import sdg from "@/assets/sdg.png";
  const openMail = (mailto) => {
    window.location.href = 'mailto:info@humannature.agency';
  };
</script>

<template>
  <v-container fluid class="mt-10 mb-10 mx-auto justify-center align-center" >
    <v-row no-gutters>
       <v-col cols="4" sm="4" md="4" class="ml-auto mr-0">
         <h2 class="wide">Let's <span class="green">change the world,</span></h2>
          <h2>because we can.</h2>
        <br/>
        <v-btn class="email-btn rounded-0 green" @click="openMail">
          Get In Touch
        </v-btn>
      </v-col>
       <v-col cols="2" sm="2" md="2" class="mr-auto ml-0">
          <v-img :src="sdg" fluid />
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
h2 {
  color: #FFF;
  font-size: 2.5em;
}

.email-btn {
  background-color: #09C771;
  color: #000;
}
@media (max-width: 1024px) {
  h2 {
    font-size: 0.5em;
  }
}
.email-btn {
  background-color: #09C771;
  color: #000;
}
</style>
