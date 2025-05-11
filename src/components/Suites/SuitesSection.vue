<script setup lang="ts">
    import Suite from '@/components/Suites/Suite.vue';
</script>

<template>
  <div class="suites-section">

    <div class="suites__titles">
      <h2>Voyager avec distinction</h2>
      <p>
        Profitez d’un service d’exception pensé pour votre confort, du décollage jusqu’à votre
        arrivée en France.
      </p>
    </div>

    <div class="suites__list">
        <Suite name="FlyAir" src="/assets/img/suites/flyair.png">
          <h2>La suite FlyAir - L'excellence absolue en altitude.</h2>

          <p style="margin-bottom: 32px;">Chaque instant de votre vol devient un privilège rare.</p>

          <ul>
            <li>Service buffet à volonté.</li>
            <li>Chambre avec lit double.</li>
            <li>Salon privé.</li>
            <li>Salle d'eau privée</li>
          </ul>
        </Suite>

        <Suite name="Elegance" src="/assets/img/suites/elegance.png" inverted>
          <h2>La suite FlyAir - L'excellence absolue en altitude.</h2>

          <p style="margin-bottom: 32px;">Chaque instant de votre vol devient un privilège rare.</p>

          <ul>
            <li>Service buffet à volonté.</li>
            <li>Chambre avec lit double.</li>
            <li>Salon privé.</li>
            <li>Salle d'eau privée</li>
          </ul>
        </Suite>

        <Suite name="Essentielle" src="/assets/img/suites/essentielle.png">
          <h2>La suite FlyAir - L'excellence absolue en altitude.</h2>

          <p style="margin-bottom: 32px;">Chaque instant de votre vol devient un privilège rare.</p>

          <ul>
            <li>Service buffet à volonté.</li>
            <li>Chambre avec lit double.</li>
            <li>Salon privé.</li>
            <li>Salle d'eau privée</li>
          </ul>
        </Suite>
    </div>

  </div>
</template>

<style scoped lang="scss">
    .suites-section {
      padding-block: 250px;
      padding-inline: 160px;

      color: var(--secondary);

      h2 {
        color: var(--secondary);
      }

      background-color: #F3EDE5;

      &.suites__titles {

      }

      .suites__list {
        margin-top: 150px;
        display: flex;
        flex-direction: column;
        gap: 128px;
      }
    }
</style>
