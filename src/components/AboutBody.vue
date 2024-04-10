<script setup lang="ts">
import homeImage from "@/assets/home-image-one.png";
import jess from "@/assets/jess.png";
import jade from "@/assets/jade.png";
import both from "@/assets/both.png";

import brands from "@/assets/brands-no-gutters.png";

  const openMail = () => {
    window.location.href = 'mailto:info@humannature.agency';
  };
</script>

<template>
  <v-container fluid class="services mt-10 mx-auto mb-10 justify-center align-center" >
    <v-row class="pl-15 pr-15">
       <v-col cols="12" sm="12" md="12">
        <h1>About us</h1>
      </v-col>
    </v-row>
    <v-row class="para align-content-sm pl-15 pr-15">
        <v-col cols="6" class="ml-auto services-text mb-0">
         <p>
            With over 20 years of international experience, honed across advertising agencies,
            tech startups, and social impact ventures, we've helped brands win recognition
            (and awards), drive sales, build loyalty, and educate audiences. Through our work,
            we've harnessed the transformative nature of storytelling and communication to
            drive positive change and impact behaviour.
        </p>
      </v-col>
       <v-col cols="6" class="mr-auto services-text mb-0">
         <p>
            So, why the pivot to our own venture? Well, we really, really give a damn.
        </p>

        <p>
            We care about people (Humans) and the planet (Nature)—human rights, animal rights,
            sustainability, diversity and representation, fair opportunity and education. And
            we are committed to leveraging our expertise to drive meaningful change in these areas.
        </p>
      </v-col>
    </v-row>
    </v-container>
    <v-container fluid>
    <v-row class="para pl-15 pr-15">
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
    <v-row class="para mt-10 pl-15 pr-15 text-center">
        <v-col cols="12" xs="12" sm="12" md="12" class="mr-auto ml-auto">
            <p>
                Our vision is a world where our talents and network are used for good—positively
                influencing behaviour and contributing to a better world by building better brands.
            </p>
            <br/>
            <p>
                <b>The world is changed by big ideas and people brave enough to bring them to life.
                As creative problem solvers, we have the power to do that, and we can change it for
                the better. So let’s do that.</b>
            </p>
        </v-col>
    </v-row>
    <v-row class="para pl-15 pr-15">
        <v-col cols="12" sm="12" md="12" class="mx-auto">
        <h1>Our values</h1>
      </v-col>
    </v-row>
    <v-row class="para pl-15 pr-15">
      <v-col cols="12" sm="12" md="3">
        <h3>Work with courage</h3>
        <p>Act decisively, with courage and resolve, because changing the world needs bravery and action.</p>
      </v-col>
      <v-col cols="12" sm="12" md="3" class="ml-auto">
        <h3>Craft excellence</h3>
        <p>
            Masterful design and copywriting elevate brand assets beyond aesthetics, driving the very
            impact the brand aspires to. #PixelPerfect
        </p>
      </v-col>
      <v-col cols="12" sm="12" md="3" class="ml-auto">
        <h3>Drive impact</h3>
        <p>Make change through empathy, consideration, creativity, true data and strategy.</p>
      </v-col>
    </v-row>
    <v-row class="para pl-15 pr-15">
      <v-col cols="12" sm="12" md="3">
        <h3>Approach challenges with curiosity</h3>
        <p>Challenge norms, embrace risks, and view setbacks as learning opportunities. Experimentation fuels growth. #NotBusinessAsUsual</p>
      </v-col>
      <v-col cols="12" sm="12" md="3" class="ml-auto">
        <h3>Integrity is non-negotiable</h3>
        <p>Foster collective strength through collaboration, honesty, empathy, transparency and respect.</p>
      </v-col>
      <v-col cols="12" sm="12" md="3" class="ml-auto">
        &nbsp;
      </v-col>
    </v-row>
  </v-container>
  <v-container fluid>
    <v-row class="para pl-15 pr-15">
      <v-col cols="12" sm="12" md="12">
            <h3>We’ve worked with some of the world’s biggest (and smallest) brands and agencies across the globe:</h3>
        </v-col>
    </v-row>
    <v-row class="para pl-15 pr-15">
      <v-col cols="12" sm="12" md="12" class="ml-auto mr-auto mb-10">
          <v-img :src="brands" />
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
.services {
  color: #fff;
}
h1 {
  font-size: 5em;
  padding-bottom:20;
}
h3 {
    font-size: 1.5em;
    color: #fff;
    font-weight:bold;
    padding-bottom:25px;
}
.nav-btn {
  background-color: #09C771;
  color: #000;
}
.services-text {
  font-size: 1em;
}
.services-blocks {
  background-color: #111111;
}
ul > li {
    margin-left: 20px;
}
@media (max-width: 1024px) {
  h1 {
    font-size: 3em;
  }
  .services-text {
    font-size: 0.5em;
  }
}
</style>
