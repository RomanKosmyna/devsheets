<script setup lang="ts">
import MainHeader from '@/components/MainHeader.vue';
import BackgroundWrapper from '@/components/BackgroundWrapper.vue';
import MainWrapper from '@/components/MainWrapper.vue';
</script>

<template>
  <BackgroundWrapper>
    <MainHeader />
    <MainWrapper>
      <div class="about">
        <p>About Page</p>
      </div>
    </MainWrapper>
  </BackgroundWrapper>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: calc(100vh - 80px);
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 30px;
  }
}
</style>
