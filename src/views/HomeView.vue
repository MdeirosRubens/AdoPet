<template class>
    <HeaderView />
    <section class="container-home">
        <div class="logo">
            <img src="@/assets/imgs/logos/logo_branco.svg" alt="">
        </div>
        <div class="welcome-text">
            <span class='welcome-text__span'>Boas-vindas!</span>
        </div>
        <div class="desc-text">
            <p class="desc-text__desc">
                Que tal mudar sua vida adotando seu novo melhor amigo? Vem com a gente!
            </p>
        </div>
        <div class="botoes">
            <button class="btn-large">
                Já tenho conta
            </button>
            <button class="btn-large">
                Quero me cadastrar
            </button>
        </div>
        <div class="cat_dog">
            <img class="cat_dog__img" src="@/assets/imgs/cat_dog.svg" alt="Ilustração de Gato e Cachorro">
        </div>
    </section>
</template>

<script lang="ts">

import { defineComponent } from "vue";
import HeaderView from "./HeaderView.vue";

export default defineComponent({
    name: 'HomeView',
    components: { HeaderView }
});
</script>

<style>
body {
    background-color: #3772FF;
    color: #fff;

}

.container-home {
    font-family: 'Poppins', sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
    position: fixed;
    top: 15%;
    z-index: 10;
    background-image: url(@/assets/imgs/background/Forma_2.png);
    background-repeat: no-repeat;
    background-position: right;
}

.welcome-text__span {
    font-size: 1.625em;
    font-weight: 500;
    line-height: 3em;
}

.desc-text__desc {
    font-weight: 400;
    line-height: 1.5em;
    text-align: center;
    height: 4.5rem;
}

.botoes {
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
}

.cat_dog__img {
    margin-top: 1.875rem;
}
</style>