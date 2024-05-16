<script setup lang="ts">

  import sdg from "@/assets/sdg.png";
  const openMail = (mailto) => {
    window.location.href = 'mailto:info@humannature.agency';
  };
</script>

<template>
  <v-container fluid class="mt-10 mb-10 mx-auto justify-center" >
    <v-row no-gutters class="pl-5 pr-5">
       <v-col cols="12" sm="12" md="6" class="pl-15 pr-15 mt-15 pt-15 mb-10
         align-center">
         <h1 class="dark medium">Let's <span class="green dark">change the
             world,</span></h1>
          <h1 class="dark medium">because we can.</h1>
        <br/>
        <v-btn class="email-btn rounded-0 green" @click="openMail">
          Get In Touch
        </v-btn>
      </v-col>
       <v-col cols="12" sm="12" md="6" class="align-center pl-10 pr-10 mt-10 mb-10">
          <v-img :src="sdg" :width="300" class="mx-auto"/>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
h1 {
  font-size: 4em;
  line-height: 1em;
  color: #FFF;
}

.email-btn {
  background-color: #09C771;
  color: #000;
}
@media (max-width: 1024px) {
  h1 {
    font-size: 2em;
  }
}
.email-btn {
  background-color: #09C771;
  color: #000;
}
</style>
