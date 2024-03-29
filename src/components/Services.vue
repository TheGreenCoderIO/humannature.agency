<script setup lang="ts">
  import homeImage from "@/assets/home-image-one.png";

  const openMail = (mailto) => {
    window.location.href = 'mailto:info@humannature.agency';
  };
</script>

<template>
  <v-container fluid class="services mt-10 mx-auto mb-10 justify-center align-center" >
    <v-row no-gutters>
       <v-col cols="12" sm="12" md="6" class="mx-auto mt-10 mb-10">
        <h1>Services</h1>
      </v-col>
    </v-row>
    <v-row no-gutters class="para">
      <v-col cols="2" class="ml-auto mb-15" fluid>
          <v-img :src="homeImage" />
      </v-col>
       <v-col cols="2" class="mt-15 mr-3 ml-3">
          <v-img :src="homeImage"/>
      </v-col>
       <v-col cols="2" class="mr-auto services-text mb-0">
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
    <v-row no-gutters class="para mt-10">
      <v-col cols="2" class="ml-auto services-blocks pt-5 pb-10 pr-5 pl-5" fluid>
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
      <v-col cols="2" class="mr-3 ml-3 services-blocks pt-5 pb-10 pr-5 pl-5" fluid>
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
      <v-col cols="2" class="mr-auto services-blocks pt-5 pb-10 pr-5 pl-5" fluid>
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
  h1 {
    font-size: 3em;
  }
  .services-text {
    font-size: 0.5em;
  }
}
</style>
