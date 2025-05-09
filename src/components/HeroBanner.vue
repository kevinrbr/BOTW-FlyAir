<script setup lang="ts">
import Button from '@/components/Button.vue';

</script>

<template>
  <div class="hero">
    <!-- <img src="@/assets/herobg.png" /> -->
    <h1 class="hero__title">L'envol à la Française</h1>
    <div>
        <Button label="Cap sur la France : où commence votre voyage ?" />
    </div>
  </div>
</template>

<style scoped lang="scss">
.hero {
    display: flex;
    height: 125dvh;
    align-items: center;
    flex-direction: column;
    gap: 50px;
    background: var(--color-background);

    &__title {
        margin-top: calc(50dvh - 86px);
    }
}

</style>