<template>
    <div>
        <h3>{{ category.name }}</h3>
    </div>
</template>

<script setup lang="ts">
const { category } = defineProps<{
    category: {
        name: string
        logo: string
    }
}>()

</script>

<style></style>
