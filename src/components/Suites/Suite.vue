<script setup lang="ts">
    const props = defineProps<{
        src: string
        name: string
        inverted?: boolean
    }>();
</script>

<template>
    <div class="suite-card" :class="{ 'suite-card--inverted': inverted }">
        <div class="card__img">
            <img :src="src" :alt="name" />
        </div>

        <div class="card__content">
            <slot />
        </div>
    </div>
</template>

<style scoped lang="scss">
    .suite-card {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 10vw;
        width: 100%;

        &--inverted {
            flex-direction: row-reverse;
        }

        .card__img {
            img {}
        }

        .card__content {}
    }
</style>