<template>
    <div class="monuments">
        <div class="container">
            <h2 class="monuments__title">Découvrir une culture</h2>
            <p class="monuments__text">Plongez dans l’art de vivre à la française, entre patrimoine, raffinement et émotions intenses.</p>
            <div class="monuments__list">
                <div class="monuments__image-container">
                    <img src="@/assets/monuments/mo-1.png" />
                </div>
                <div class="monuments__image-container">
                    <img src="@/assets/monuments/mo-2.png" />
                </div>
                <div class="monuments__image-container">
                    <img src="@/assets/monuments/mo-3.png" />
                </div>
                <div class="monuments__image-container">
                    <img src="@/assets/monuments/mo-4.png" />
                </div>
                <div class="monuments__image-container">
                    <img src="@/assets/monuments/mo-5.png" />
                </div>
                <div class="monuments__image-container">
                    <img src="@/assets/monuments/mo-6.png" />
                </div>
            </div>
            <div class="monuments__name-container">
                <span class="monuments__name">Monuments</span>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
.monuments {
    background-color: var(--secondary);
    padding: 150px 0;

    &__title {
        color: var(--color-text-secondary);
    }

    &__text {
        color: var(--color-text-secondary);
        font-size: 24px;
    }

    &__list {
        width: 100vw;
        margin-left: calc(-1 * ((100vw - 100%) / 2));
        padding: 0 16px; 
        display: flex;
        gap: 16px;
        margin-top: 200px;
        margin-bottom: 180px;
    }
    
    &__image-container {
        height: 340px;
        width: 269px;
    }

    &__name-container {
        text-align: center;
    }

    &__name {
        font-family: 'Kaftan';
        // text-align: center;
        color: var(--color-text-secondary);
        font-size: 64px;
    }
}
</style>