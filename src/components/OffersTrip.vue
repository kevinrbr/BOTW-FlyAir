<script setup lang="ts">
</script>

<template>
  <div class="offers container">
    <h2>Nos offres de voyage</h2>
    <div class="wrapper">
        <p class="offers__intro">Accédez à nos offres exclusives pour découvrir la France dans toute son élégance.</p>
        <a class="offers__link">Voir toutes les offres</a>
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
}
</style>