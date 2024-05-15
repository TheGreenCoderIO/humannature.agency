<script setup lang="ts">
  import serviceOne from "@/assets/service-one.webp";
  import serviceTwo from "@/assets/service-two.webp";

  const openMail = () => {
    window.location.href = 'mailto:info@humannature.agency';
  };
</script>

<template>
  <v-container fluid class="services mt-10 mb-10" >
    <v-row class="pl-5 pr-5">
       <v-col cols="12" sm="12" md="12" class="mx-auto mb-10">
        <h1 class="dark-medium">Services</h1>
      </v-col>
    </v-row>
    <v-row class="para pl-5 pr-5">
      <v-col cols="12" xs="12" sm="12" md="4" class="ml-auto mb-15">
          <v-img :src="serviceOne" />
      </v-col>
       <v-col cols="12" xs="12" sm="12" md="4" class="mt-10">
          <v-img :src="serviceTwo"/>
      </v-col>
       <v-col cols="12" xs="12" sm="12" md="4" class="mr-auto services-text mb-0">
         <p>Data and statistics only go so far. To <b>capture hearts, inspire
           action and change behaviour</b>, we harness the <b>power
           of storytelling</b> and
         <b>brand building</b>.</p>
        <br/>
         <p>It's the difference between facts on a page and
         creating a connected brand experience that resonates with
         stakeholders, employees and customers.</p>
        <v-btn class="nav-btn rounded-0 mt-5" @click="openMail">
          Get In Touch
        </v-btn>
      </v-col>
    </v-row>
    <v-row class="para pl-5 pr-5">
      <v-col cols="12" xs="12" sm="12" md="4" class="ml-auto">
        <div class="services-blocks pl-10 pt-10 pb-10 pr-10">
        <h2 class="dark-medium">Stroytelling for impact</h2>
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
        </div>
      </v-col>
      <v-col cols="12" xs="12" sm="12" md="4" class="ml-auto mr-auto">
        <div class="services-blocks pl-10 pt-10 pb-10 pr-10">
        <h2 class="dark-medium">Brand development</h2>
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
        </div>
      </v-col>
      <v-col cols="12" xs="12" sm="12" md="4" class="mr-auto">
        <div class="services-blocks pl-10 pt-10 pb-10 pr-10">
        <h2 class="dark-medium">Content & campaigns</h2>
        <br/>
        <ul>
          <li>Integrated campaigns</li>
          <li>Social media campaigns</li>
          <li>Google ads campaigns</li>
          <li>Email campaigns</li>
          <li>Creative concept</li>
          <br/>
          <br/>
        </ul>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
.nav-btn {
  background-color: #09C771;
  color: #000;
}
.services-text {
  font-size: 1em;
}
.services-blocks {
  background-color: #111111;
  font-size: 1em;
}


ul > li {
    margin-left: 20px;
}
</style>
