<script lang="ts">
import { ref, watch, onMounted } from 'vue';

export default {
  setup() {
    const words = ref(['change-makers', 'chance-takers','brave', 'kind', 'rebels', 'dreamers', 'doers', 'challengers', 'innovators']); // Your list of words

    return {
      words,
    };
  }
};
</script>

<template>
  <v-container fluid class="landing mt-10 mb-10 ml-0 mr-0 text-left" >
    <v-row class="mt-10 mb-10">
       <v-col cols="12" sm="12" md="12" class="pl-10 pr-10 pt-15 mt-15">
         <h1 class="wide dark header not-bold">We work with the </h1>
      </v-col>
       <v-col cols="12" sm="12" md="12" class="pb-15 mb-15 animation-style">
         <ul id="changeMaker" class="animation dark green">
           <li v-for="word in words" class="cm"><h1 class="header"><b>{{ word
                 }}.</b></h1></li>
         </ul>
      </v-col>
       <v-col cols="12" sm="12" md="6">
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>

.landing {
  width: 100%;
  color: white;
  background-image: url('@/assets/about-header.webp');
  background-size: cover;
}

.animation {
  list-style: none;
  padding: 0;
  margin: 0;
}

.animation-style {
  position: relative;
}

.animation-style li {
  list-style: none;
  width: 70%;
  opacity: 0;
  position: absolute;
  left: 30%;
  text-align: right !important;
  display: table;
  transform: translate(-50%, -50%);
}

.cm {
  animation: fadeIn 18s ease infinite;
}

.animation li.active {
  opacity: 1;
}
.animation li:nth-child(1) {
  animation-delay: 0s;
}

.animation li:nth-child(2) {
  animation-delay: 2s; /* Adjust the delay as needed */
}

.animation li:nth-child(3) {
  animation-delay: 4s; /* Adjust the delay as needed */
}

.animation li:nth-child(4) {
  animation-delay: 6s; /* Adjust the delay as needed */
}
.animation li:nth-child(5) {
  animation-delay: 8s; /* Adjust the delay as needed */
}
.animation li:nth-child(6) {
  animation-delay: 10s; /* Adjust the delay as needed */
}
.animation li:nth-child(7) {
  animation-delay: 12s; /* Adjust the delay as needed */
}
.animation li:nth-child(8) {
  animation-delay: 14s; /* Adjust the delay as needed */
}

.animation li:last-child {
  animation-delay: 16s; /* Adjust the delay as needed */
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  10% {
    opacity: 1;
  }
  20% {
    opacity: 0;
  }
  30% {
    opacity: 0;
  }
  40% {
    opacity: 0;
  }
  50% {
    opacity: 0;
  }
  60% {
    opacity: 0;
  }
  70% {
    opacity: 0;
  }
  80% {
    opacity: 0;
  }
  90% {
    opacity: 0;
  }
  100% {
    opacity: 0;
  }
}

@media (max-width: 1024px) {
.animation-style li {
  list-style: none;
  width: 90%;
  opacity: 0;
  position: absolute;
  left: 40%;
  text-align: right !important;
  display: table;
  transform: translate(-50%, -50%);
}
}
</style>
