<script setup lang="ts">
const props = defineProps<{
  iconName: string;
  label: string;
}>();
</script>

<template>
  <div class="circle-icon container">
    <div class="circle-icon__icon">I</div>
    <span class="circle-icon__text">{{ label }}</span>
  </div>
</template>

<style scoped lang="scss">
.circle-icon {
    &__icon {
        background-color: var(--secondary);
        height: 40px;
        width: 40px;
        border-radius: 100%;
    }
    &__text {
        font-size: 14px;
        color: var(--color-text)
    }
}
</style>