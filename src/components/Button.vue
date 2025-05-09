<script setup lang="ts">
import type { ButtonVariant } from '@/types/ButtonType'

const props = withDefaults(defineProps<{
  label: string;
  variant?: ButtonVariant;
}>(), {
  variant: 'primary',
});

</script>

<template>
    <button :class="`btn btn--${variant}`">{{ label }}</button>
</template>

<style scoped lang="scss">
.btn {
  padding: 12px 30px;
  border-radius: 24px;
  font-family: 'Suisse Intl';
  cursor: pointer;

  &--primary {
    background-color: var(--primary);
    color: var(--secondary);
    border: 1px solid var(--secondary);
  }
}
</style>
