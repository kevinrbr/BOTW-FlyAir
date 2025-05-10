<script setup lang="ts">
const props = defineProps<{
  icon: string;
  label: string;
}>();
</script>

<template>
  <div class="circle-icon">
    <div class="circle-icon__icon">
      <img src="@/assets/icons/arrow.svg" />
    </div>
    <span class="circle-icon__text">{{ label }}</span>
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
    }
}
</style>