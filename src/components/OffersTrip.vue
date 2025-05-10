<script setup lang="ts">
import CircleIconLink from '@/components/CircleIconLink.vue';
import TripCardVue from '@/components/TripCard.vue';

</script>

<template>
  <div class="offers container">
    <h2>Nos offres de voyage</h2>
    <div class="wrapper">
        <p class="offers__intro">Accédez à nos offres exclusives pour découvrir la France dans toute son élégance.</p>
        <a class="offers__link">Voir toutes les offres</a>
    </div>
    <div class="offers__circles">
        <CircleIconLink is-arrow label="Aller simple"/>
        <CircleIconLink label="Aller-retour"/>
    </div>
    <div class="trips-wrapper">
        <div class="column left">
            <TripCardVue 
            image="src/assets/marseille.png" 
            city="Marseille"
            region="Provence-Alpes-Côte d'Azur"
            price="658"
            />
            <TripCardVue 
            image="src/assets/marseille.png" 
            city="Paris"
            region="Île-de-France"
            price="712"
            />
        </div>
        <div class="column right">
            <TripCardVue 
            image="src/assets/marseille.png" 
            city="Annecy"
            region="Auvergne-Rhône-Alpes"
            price="562"
            />
            <TripCardVue 
            image="src/assets/marseille.png" 
            city="Bordeaux"
            region="Nouvelle-Aquitaine"
            price="524"
            />
        </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.trips-wrapper {
    margin: 100px 0;
    display: flex;
    align-items: flex-start;
    flex-wrap: wrap;
    gap: 16px;
    width: 100%;
}

.column {
  display: flex;
  width: 100%;
  gap: 16px;
}

.left {
    justify-content: flex-start;
}

.right {
    justify-content: flex-end;
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