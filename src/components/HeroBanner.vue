<script setup lang="ts">
import Button from '@/components/Button.vue';

</script>

<template>
  <div class="hero">
    <img src="@/assets/herobg.png" />
    <h1 class="hero__title">L'envol à la Française</h1>
    <div>
        <Button label="Cap sur la France : où commence votre voyage ?" />
    </div>
  </div>
</template>

<style scoped lang="scss">
.hero {
  position: relative;
    display: flex;
    height: 125dvh;
    align-items: center;
    flex-direction: column;
    gap: 50px;
    background: var(--color-background);
    width: 100%;

    img {
      position: absolute;
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      object-fit: cover;
      z-index: 0;
      filter: brightness(0.5);
    }

    &__title {
        margin-top: calc(50dvh - 86px);
    }

    h1, div {
      position: relative;
      z-index: 1;
    }
}

</style>