<script setup lang="ts">
import CircleIconLink from '@/components/CircleIconLink.vue'
import { computed } from 'vue'

const props = defineProps<{
  image: string
  city: string
  region: string
  price: string
}>()

const priceText = computed(() => `Dès ${props.price}€*`)
</script>

<template>
  <div class="offer-card">
    <div class="offer-card__image-wrapper">
      <img class="offer-card__image" :src="image" :alt="city" />
      <div class="offer-card__badge">
        <CircleIconLink :label="priceText" is-white />
      </div>
    </div>
    <div class="offer-card__info">
      <h3 class="offer-card__city">{{ city }}</h3>
      <p class="offer-card__region">{{ region }}</p>
    </div>
  </div>
</template>

<style scoped lang="scss">
.offer-card {
  position: relative;
  width: 412px;

  &__image-wrapper {
    position: relative;
    width: 100%;
    height: 100%;
    overflow: hidden;

    .offer-card__image {
      width: 100%;
      height: 100%;
      filter: brightness(0.75);
    }

    .offer-card__badge {
      position: absolute;
      top: 20px;
      left: 20px;
      display: flex;
      align-items: center;
      gap: 10px;
      color: white;
      font-weight: bold;
      font-size: 16px;
    }
  }

  &__info {
    padding: 20px;
    position: absolute;
    bottom: 0;

    .offer-card__city {
      font-weight: bold;
      font-size: 18px;
      margin: 0;
      font-size: 16px;
      color: var(--primary);
      font-family: 'Suisse Intl';
      font-weight: bold;
    }

    .offer-card__region {
      margin: 0;
      color: #444;
      font-size: 16px;
      color: var(--primary);
      font-family: 'Suisse Intl';
    }
  }
}
</style>
