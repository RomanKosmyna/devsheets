<template>
    <main>
        <slot />
    </main>
</template>

<style>
main {
    width: 100%;
    padding: 0 1.25rem;
}

@media (min-width: 1024px) {
    main {
        display: flex;
        justify-content: center;
    }
}
</style>
