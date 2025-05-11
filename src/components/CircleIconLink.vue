<script setup lang="ts">
import { computed } from 'vue';

const props = withDefaults(defineProps<{
  label: string;
  isArrow?: boolean;
  isWhite?: boolean;
}>(), {
  isArrow: false,
  isWhite: false
});

const iconUrl = computed(() => props.isArrow ? "/assets/icons/arrow.svg" : "/assets/icons/swap.svg")
</script>

<template>
  <div class="circle-icon">
    <div class="circle-icon__icon">
      <img :src="iconUrl" />
    </div>
    <span :class="['circle-icon__text', { 'is-white': isWhite }]">
      {{ label }}
    </span>
  </div>
</template>

<style scoped lang="scss">
.circle-icon {
  display: flex;
  align-items: center;

    &__icon {
        background-color: var(--secondary);
        height: 40px;
        width: 40px;
        border-radius: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        margin-right: 20px;
    }

    &__text {
        font-size: 14px;

        &.is-white {
          color: var(--color-text-secondary);
        }
    }
}
</style>