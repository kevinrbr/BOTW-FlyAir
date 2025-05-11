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
    margin-top: 100px;
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
    padding-block: 350px;
    background-color: #F3EDE5;

    &__intro {
        font-size: 24px;
        font-family: 'Suisse Intl';
        color: var(--secondary);
    }

    &__link {
        text-decoration: underline;
        color: var(--secondary);
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