<script lang="ts">
import { ref, computed, onMounted, onBeforeUnmount } from 'vue';

export default {
  setup() {
    const words = ref(['brave', 'kind', 'rebels', 'dreamers', 'doers',
    'challengers', 'innovators', 'change-makers', 'chance-takers']); // Your list of words
    const currentIndex = ref(0);

    const currentWord = computed(() => words.value[currentIndex.value]);

    let intervalId;

    onMounted(() => {
      // Start changing the word every 2 seconds
      intervalId = setInterval(() => {
        currentIndex.value = (currentIndex.value + 1) % words.value.length;
      }, 2000);
    });

    onBeforeUnmount(() => {
      // Clear the interval when the component is destroyed to prevent memory leaks
      clearInterval(intervalId);
    });

    return {
      currentWord
    };
  }
};
</script>

<template>
  <v-container fluid class="landing mt-10 mb-10 justify-center text-center align-center" >
    <v-row no-gutters>
       <v-col cols="12" sm="12" md="12" class="pl-15 pr-15 pt-15 pb=15 mt-15 mb-15">
         <h1 class="wide">We work with the </h1>
         <transition name="rotate-transition" mode="out-in">
           &emsp;<h1 :key="currentWord" class="wide green">{{ currentWord }}.</h1>
         </transition>
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
.word {
  position: absolute;
  width: 100%;
  left: 0;
  top: 0;
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
