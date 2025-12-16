<script setup lang="ts">
import MainHeader from '@/components/MainHeader.vue';
import TheWelcome from '../components/TheWelcome.vue'
import BackgroundWrapper from '@/components/BackgroundWrapper.vue';
import MainWrapper from '@/components/MainWrapper.vue';
</script>

<template>
  <BackgroundWrapper>
    <MainWrapper>
      <MainHeader />
      <TheWelcome />
    </MainWrapper>
  </BackgroundWrapper>
</template>

<style>
main {
  width: 100%;
  padding: 0 1.25rem;
}
</style>
