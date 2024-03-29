<script setup lang="ts">
  import homeImage from "@/assets/home-image-one.png";

  const openMail = () => {
    window.location.href = 'mailto:info@humannature.agency';
  };
</script>

<template>
  <v-container fluid class="services mt-10  mx-auto mb-10 justify-center align-center" >
    <v-row class="pl-15 pr-15">
       <v-col cols="12" sm="12" md="12" class="mx-auto mt-10 mb-10">
        <h1>Services</h1>
      </v-col>
    </v-row>
    <v-row class="para pl-15 pr-15">
      <v-col cols="12" xs="12" sm="12" md="4" class="ml-auto mb-15">
          <v-img :src="homeImage" />
      </v-col>
       <v-col cols="12" xs="12" sm="12" md="4" class="mt-10">
          <v-img :src="homeImage"/>
      </v-col>
       <v-col cols="12" xs="12" sm="12" md="4" class="mr-auto services-text mb-0">
         <p>Data and statistics only go so far. To <strong>capture hearts, inspire
           action and change behaviour</strong>, we harness the <strong>power
           of storytelling</strong> and
         <strong>brand building</strong>.</p>
        <br/>
         <p>It's the difference between facts on a page and
         creating a connected brand experience that resonates with
         stakeholders, employees and customers.</p>
        <v-btn class="nav-btn rounded-0" @click="openMail">
          Get In Touch
        </v-btn>
      </v-col>
    </v-row>
    <v-row class="para pl-15 pr-15">
      <v-col cols="12" xs="12" sm="12" md="4"class="mt-10 services-blocks">
        <h2>Stroytelling for impact</h2>
        <br/>
        <ul>
          <li>Visualising ESG reporting
            <ul>
              <li>Video</li>
              <li>Animation</li>
              <li>Infographics</li>
            </ul>
          </li>
          <li>Workshops
            <ul>
              <li>Uncovering and amplifying your impact</li>
            </ul>
          </li>
          <li>Employee branding</li>
        </ul>
      </v-col>
      <v-col cols="12" xs="12" sm="12" md="4" class="mt-10 services-blocks">
        <h2>Brand development</h2>
        <br/>
        <ul>
          <li>Brand identity & guidelines</li>
          <li>Brand messaging</li>
          <li>Tone of Voice development</li>
          <li>Communication strategy</li>
          <li>Sustainable UX/UI design</li>
          <li>Sustainable web design</li>
          <li>SEO</li>
        </ul>
      </v-col>
      <v-col cols="12" xs="12" sm="12" md="4" class="mt-10 services-blocks">
        <h2>Content & campaigns</h2>
        <br/>
        <ul>
          <li>Integrated campaigns</li>
          <li>Social media campaigns</li>
          <li>Google ads campaigns</li>
          <li>Email campaigns</li>
          <li>Creative concept</li>
        </ul>
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
}
</style>
