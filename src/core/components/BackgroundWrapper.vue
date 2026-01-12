<script setup lang="ts">
defineProps<{ bg: string }>();
</script>

<template>
    <div class="wrapper">
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
    background: rgba(0, 16, 17);
    backdrop-filter: blur(6px);
}
</style>
