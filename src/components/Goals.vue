<script setup lang="ts">

  import sdg from "@/assets/sdg.png";
  const openMail = (mailto) => {
    window.location.href = 'mailto:info@humannature.agency';
  };
</script>

<template>
  <v-container fluid class="mt-10 mb-10 mx-auto justify-center align-center" >
    <v-row no-gutters class="pl-15 pr-15">
       <v-col cols="12" sm="12" md="6" class="pl-15 pr-15 mt-10 mb-10">
         <h2 class="wide">Let's <span class="green">change the world,</span></h2>
          <h2>because we can.</h2>
        <br/>
        <v-btn class="email-btn rounded-0 green" @click="openMail">
          Get In Touch
        </v-btn>
      </v-col>
       <v-col cols="12" sm="12" md="6" class="align-center pl-15 pr-15 mt-10 mb-10">
          <v-img :src="sdg" :width="300" class="mx-auto"/>
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
    font-size: 2em;
  }
}
.email-btn {
  background-color: #09C771;
  color: #000;
}
</style>
