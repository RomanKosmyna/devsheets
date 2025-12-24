<script setup lang="ts">
import BackgroundWrapper from '@/components/BackgroundWrapper.vue';
import MainHeader from '@/components/MainHeader.vue';
import bg from "../assets/docs-bg.jpg";
</script>

<template>
    <BackgroundWrapper :bg="bg">
        <MainHeader />
        <MainWrapper>
            <div class="sheets">
                <p>Sheets Page</p>
            </div>
        </MainWrapper>
    </BackgroundWrapper>
</template>

<style>
@media (min-width: 1024px) {
    .sheets {
        min-height: calc(100vh - 80px);
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 30px;
    }
}
</style>
