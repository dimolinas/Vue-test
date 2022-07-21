<script setup>
import WelcomePage from './components/WelcomePage.vue';
import PageOne from './components/PageOne.vue';
import PageSecond from './components/PageSecond.vue';

const routes = {
  '/': WelcomePage,
  '/1': PageOne
}


</script>

<template>
  <WelcomePage/>
</template>

<style scoped>
</style>
