<<<<<<< Updated upstream
<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
=======
<script setup lang="ts">
import MainHeader from '@/components/MainHeader.vue';
import BackgroundWrapper from '@/components/BackgroundWrapper.vue';
import MainWrapper from '@/components/MainWrapper.vue';
import bg from "../assets/about-bg.jpg";
</script>

<template>
  <BackgroundWrapper :bg="bg">
    <MainHeader />
    <MainWrapper>
      <div class="about">
        <p>About Page</p>
      </div>
    </MainWrapper>
  </BackgroundWrapper>
>>>>>>> Stashed changes
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
