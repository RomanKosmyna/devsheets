<script setup lang="ts">
defineProps<{ bg: string }>();
</script>

<template>
    <div class="wrapper" :style="{ backgroundImage: `url(${bg})` }">
        <slot />
    </div>
</template>

<style>
.wrapper {
    width: 100%;
    height: 100vh;
    position: relative;
    background-size: cover;
    background-position: center;
    z-index: 0;
}

.wrapper::before {
    content: "";
    position: absolute;
    inset: 0;
    z-index: -1;
    background: rgba(0, 0, 0, 0.5);
    backdrop-filter: blur(6px);
}
</style>
