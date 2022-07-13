<template>
    <div class="card">
        <div class="card__picture">
            <picture>
                <img src="@/assets/imgs/card-profiles/dunga.png" alt="Foto do cachorro Dunga">
            </picture>
        </div>
        <div class="card__infos">
            <div class="name">
                <h1>Dunga</h1>
            </div>
            <div class="about">
                <p>2 anos</p>
                <p>Porte pequeno</p>
                <p>Calmo e educado</p>
            </div>
            <div class="info">
                <address class="info__adress">Rio de Janeiro (RJ)</address>
                <router-link class="info__link">
                    <img src="@/assets/imgs/icons/message-card.png" alt="">
                    <p>
                        Falar com responsável
                    </p>
                </router-link>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "ItemCard"
})

</script>

<style>
.card {
    width: 100%;
    height: 12.063rem;
    background-color: #F7F7F7;
    display: flex;
    justify-content: space-evenly;
    font-family: 'Poppins';
}

.card__picture {
    display: flex;
    align-items: center;
}

.card__infos {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}

.name {
    font-weight: 600;
    color: #3772FF;
    line-height: 1.25em;

}

.about {
    font-size: 0.875em;
    color: #737380;
    line-height: 1.25em;
}

.about p {
    padding: 0.125rem;
}

.info {
    color: #737380;
    line-height: 1.25em;
}

.info__adress {
    font-size: 0.75em;
    margin-bottom: 0.313rem;
}

.info__link {
    font-size: 0.625em;
    display: flex;
}

.info__link p {
    padding-left: 0.625rem;
}
</style>