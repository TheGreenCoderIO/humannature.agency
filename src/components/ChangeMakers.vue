<script lang="ts">
import { ref, watch, onMounted } from 'vue';

export default {
  setup() {
    const words = ref(['brave', 'kind', 'rebels', 'dreamers', 'doers',
    'challengers', 'innovators', 'change-makers', 'chance-takers']); // Your list of words

    return {
      words,
    };
  }
};
</script>

<template>
  <v-container fluid class="landing mt-10 mb-10 justify-center text-center align-center" >
    <v-row class="mt-10 mb-10">
       <v-col cols="12" sm="12" md="12" class="pl-15 pr-15 pt-15 mt-15">
         <h1 class="wide">We work with the </h1>
      </v-col>
       <v-col cols="12" sm="12" md="12" class="pl-15 pr-15 pb-15 mb-15">
         <ul id="changeMaker" class="animation  animation-style green">
           <li v-for="word in words" class="cm"><h1>{{ word }}.</h1></li>
         </ul>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
h1 {
  font-size: 5em;
}
h2 {
  font-size: 1.5em;
}
.landing {
  width: 100%;
  padding: 0;
  margin: 0;
  color: white;
  background-image: url('@/assets/background-one.png');
}
.animation {
  list-style: none;
  padding: 0;
  margin: 0;
}

.animation-style li {
  list-style: none;
  opacity: 0;
  position: absolute;
  left: 50%;
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
  h1 {
    font-size: 3em;
  }
  h2 {
    font-size: 1em;
  }
}
</style>
