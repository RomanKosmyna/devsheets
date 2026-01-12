<script setup lang="ts">
import BackgroundWrapper from '@/core/components/BackgroundWrapper.vue';
import MainHeader from '@/core/components/MainHeader.vue';
import MainWrapper from '@/core/components/MainWrapper.vue';
import bg from "@/assets/docs-bg.jpg";
import CategoryList from './CategoryList.vue';
import SheetsHero from './SheetsHero.vue';

</script>

<template>
    <BackgroundWrapper :bg="bg">
        <MainHeader />
        <MainWrapper>
            <div class="sheets">
                <SheetsHero />
                <CategoryList />
            </div>
        </MainWrapper>
    </BackgroundWrapper>
</template>

<style>
.sheets {
    width: 100%;
    max-width: 1440px;
    min-height: calc(100vh - 80px);
}
</style>
