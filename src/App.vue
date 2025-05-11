<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router';
import Button from '@/components/Button.vue';
</script>

<template>
  <header>
      <nav class="nav-left">
        <RouterLink to="/">Acheter un billet</RouterLink>
        <RouterLink to="/about">Informations</RouterLink>
        <RouterLink to="/about">Nous contacter</RouterLink>
      </nav>
      <div class="logo-wrapper">
        <img class="logo" alt="flyair logo" src="@/assets/logo.svg" />
      </div>
      <Button label="Espace connexion"/>
  </header>

  <RouterView />
</template>

<style scoped lang="scss">
header {
  position: absolute;
  top: 0;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px;
  border-bottom: 1px solid var(--primary);
  z-index: 999;

  .nav-left {
    font-family: 'Suisse Intl';
    flex: 1;
    display: flex;
    gap: 20px;

    & {
      color: var(--color-text-secondary);
    }
  }

  .logo-wrapper {
    flex: 0;
    text-align: center;
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    margin-top: 8px;
  }
}
</style>
