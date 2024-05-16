<script setup lang="ts">
  import logo from "@/assets/logo.svg";
  import email from "@/assets/email-icon.png";
  import instagram from "@/assets/instagram-icon.png";
  import linkedin from "@/assets/linkedin-icon.png";

</script>

<template>
    <v-container
      app 
      class="align-center justify-center container"
      width="100%" >
      <v-row justify="center" class="text-center">
        <v-col class="mx-0 px-0" cols="12">
          <img :src="logo"/>
        </v-col>
        <v-col cols="auto" class="ma-0 pa-1">
          <a href="mailto:info@humannature.agency">
            <img  :src="email" class="icon"/>
          </a>
        </v-col>
        <v-col cols="auto" class="ma-0 pa-1">
          <a href="https://www.linkedin.com/company/human-nature-agency/about/">
            <img :src="linkedin" class="icon"/>
          </a>
        </v-col>
        <v-col cols="auto" class="ma-0 pa-1">
          <a href="https://www.instagram.com/human.nature.agency">
            <img :src="instagram" class="icon"/>
          </a>
        </v-col>
        <v-col class="mx-0 px-0 copyright" cols="12">
          <p class="para">Copyright Human.Nature 2024</p>
        </v-col>
        <v-col class="mx-0 px-0" cols="12">
          <CarbonBadge :dark="true" />
        </v-col>
      </v-row>
    </v-container>
</template>

<style scoped>
.icon {
  max-height: 25px; 
}
.copyright {
  font-size: 0.5em
}
.container {
  background-color: #000;
}
</style>
