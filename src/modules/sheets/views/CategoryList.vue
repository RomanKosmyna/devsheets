<template>
    <div>
        <CategoryItem v-for="category in categories" :key="category.name" :category="category" />
    </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import CategoryItem from './CategoryItem.vue';

const categories = ref([
    {
        name: "CRM",
        logo: "",
    },
    {
        name: "Frontend",
        logo: "",
    }
]);
</script>

<style scoped></style>
