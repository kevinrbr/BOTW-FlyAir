<script setup lang="ts">
import CircleIconLink from '@/components/CircleIconLink.vue';

</script>

<template>
  <div class="offers container">
    <h2>Nos offres de voyage</h2>
    <div class="wrapper">
        <p class="offers__intro">Accédez à nos offres exclusives pour découvrir la France dans toute son élégance.</p>
        <a class="offers__link">Voir toutes les offres</a>
    </div>
    <div class="offers__circles">
        <CircleIconLink icon="arrow" label="Aller simple"/>
        <CircleIconLink label="Aller-retour"/>
    </div>
  </div>
</template>

<style scoped lang="scss">
.wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.offers {
    margin-top: 350px;

    &__intro {
        font-size: 24px;
        font-family: 'Suisse Intl';
    }

    &__link {
        text-decoration: underline;
    }

    &__circles {
        display: flex;
        align-items: center; 
        justify-content: flex-start;
        gap: 50px;
        margin-top: 24px;
    }
}
</style>