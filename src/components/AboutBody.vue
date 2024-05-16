<script setup lang="ts">
import jess from "@/assets/jess.webp";
import jade from "@/assets/jade.webp";
import both from "@/assets/both.webp";

import brands from "@/assets/brands-no-gutters.png";

  const openMail = () => {
    window.location.href = 'mailto:info@humannature.agency';
  };
</script>

<template>
  <v-container fluid class="services mt-10 mb-10" >
    <v-row class="pl-5 pr-5 pt-10">
       <v-col cols="12" sm="12" md="12">
        <h1 class="dark-medium">About us</h1>
      </v-col>
    </v-row>
    <v-row class="para pl-5 pr-5 pb-10">
        <v-col cols="12" sm="12" md="6" class="ml-auto mb-0">
         <p class="para">
            With over 20 years of international experience, honed across advertising agencies,
            tech startups, and social impact ventures, we've helped brands win recognition
            (and awards), drive sales, build loyalty, and educate audiences. Through our work,
            we've harnessed the transformative nature of storytelling and communication to
            drive positive change and impact behaviour.
        </p>
      </v-col>
       <v-col cols="12" sm="12" md="6" class="mr-auto mb-0">
         <p class="para">
            So, why the pivot to our own venture? Well, we really, really give a damn.
        </p>
         <p class="para">
            We care about people (Humans) and the planet (Nature)—human rights, animal rights,
            sustainability, diversity and representation, fair opportunity and education. And
            we are committed to leveraging our expertise to drive meaningful change in these areas.
        </p>
      </v-col>
    </v-row>
    </v-container>
    <v-container fluid>
    <v-row class="para pl-5 pr-5 pb-10">
      <v-col cols="12" xs="12" sm="12" md="4" class="ml-auto mb-15">
          <v-img :src="jade" />
      </v-col>
      <v-col cols="12" xs="12" sm="12" md="4"  class="mt-10">
          <v-img :src="both"/>
      </v-col>
      <v-col cols="12" xs="12" sm="12" md="4"  class="mr-auto">
          <v-img :src="jess" />
      </v-col>
    </v-row>
    <v-row class="para mt-10 pl-5 pr-5">
        <v-col cols="12" xs="12" sm="12" md="12" class="mr-auto ml-auto">
            <p class="para">
                Our vision is a world where our talents and network are used for good—positively
                influencing behaviour and contributing to a better world by building better brands.
            </p>
            <br/>
            <p class="para">
                <b>The world is changed by big ideas and people brave enough to bring them to life.
                As creative problem solvers, we have the power to do that, and we can change it for
                the better. So let’s do that.</b>
            </p>
        </v-col>
    </v-row>
    <v-row class="para pl-5 pr-5 pt-10">
        <v-col cols="12" sm="12" md="12" class="mx-auto">
        <h1 class="dark-medium">Our values</h1>
      </v-col>
    </v-row>
    <v-row class="para pl-5 pr-5">
      <v-col cols="12" sm="12" md="3">
        <h2>Work with <span class="green dark"><b>courage</b></span></h2>
        <p class="para">Act decisively. And with courage. Changing the world needs bravery and action.</p>
      </v-col>
      <v-col cols="12" sm="12" md="3" class="ml-auto">
        <h2>Drive <span class="green dark"><b>impact</b></span></h2>
        <p class="para">Make change through empathy, consideration, creativity, true data and strategy.</p>
      </v-col>
      <v-col cols="12" sm="12" md="3" class="ml-auto">
        <h2><span class="green dark"><b>Craft</b></span> excellence</h2>
            <p class="para">
            Design and copywriting is how your audience meets your brand. Doing it with care elevates your brand  beyond aesthetics and towards impact. #PixelPerfect 
        </p>
      </v-col>
    </v-row>
    <v-row class="para pl-5 pr-5 pb-15">
      <v-col cols="12" sm="12" md="3">
        <h2>Approach challenges with <span
            class="green dark"><b>curiosity</b></span></h2>
        <p class="para">
Challenge norms, embrace risks, and view setbacks as learning opportunities. Experimentation fuels growth. #NotBusinessAsUsual</p>
      </v-col>
      <v-col cols="12" sm="12" md="3" class="ml-auto">
        <h2><span class="green dark"><b>Integrity</b></span> is non-negotiable</h2>
        <p class="para">Foster collective strength through collaboration, honesty, empathy, transparency and respect.</p>
      </v-col>
      <v-col cols="12" sm="12" md="3" class="ml-auto">
        &nbsp;
      </v-col>
    </v-row>
  </v-container>
  <v-container fluid class="text-center">
    <v-row class="para pt-15 mb-10">
      <v-col cols="12" sm="12" md="12" class="mx-auto">
            <h2 class="mx-auto">We’ve worked with some of the world’s <span class="green dark">biggest (and smallest)
                brands and agencies:</span></h2>
        </v-col>
    </v-row>
    <v-row class="para pl-5 pr-5 ml-auto align-center">
      <v-col cols="12" sm="12" md="12" class="mx-auto mb-10">
          <v-img :src="brands" class="mx-auto brands"/>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
.services-text {
  font-size: 1em;
}
.services-blocks {
  background-color: #111111;
}
.brands {
  max-width: 1319px;
}
</style>
