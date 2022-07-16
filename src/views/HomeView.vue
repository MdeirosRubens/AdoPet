<template class>
    <HeaderView />
    <main class="main">
        <section class="container-home">
            <div class="logo">
                <img class="logo_name" src="@/assets/imgs/logos/logo_branco.png" alt="">
            </div>
            <div class="welcome-text">
                <span class='welcome-text__span'>Boas-vindas!</span>
            </div>
            <div class="desc-text">
                <p class="desc-text__desc">
                    Que tal mudar sua vida adotando seu novo melhor amigo? Vem com a gente!
                </p>
            </div>
        </section>
        <section class="container-log">
            <div class="botoes">
                <button class="btn-large">
                    Já tenho conta
                </button>
                <button class="btn-large">
                    Quero me cadastrar
                </button>
            </div>
            <div class="cat_dog">
                <img class="cat_dog__img" src="@/assets/imgs/cat_dog.png" alt="Ilustração de Gato e Cachorro">
            </div>
        </section>
    </main>
    <FooterView />
</template>

<script lang="ts">

import { defineComponent } from "vue";
import HeaderView from "./HeaderView.vue";
import FooterView from "./FooterView.vue";


export default defineComponent({
    name: 'HomeView',
    components: { HeaderView, FooterView }
});
</script>

<style>
body {
    background-color: #3772FF;
    color: #fff;
}

.profilebutton {
    display: none;
}

.main {
    z-index: 10;
    background-image: url(@/assets/imgs/background/Forma_2.png);
    background-repeat: no-repeat;
    background-position: right;
}

.container-home {
    font-family: 'Poppins', sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.logo_name {
    width: 11.667rem;
    height: 2.875rem;
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

.container-log {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 30px;
}

.botoes {
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
}

.cat_dog__img {
    margin-top: 1.875rem;
    width: 247.34px;
    height: 312.77px;
}

@media (min-width: 768px) {

    .main {
        background-image: url(@/assets/imgs/background/Forma_2_alt.png);
    }

    .cat_dog__img {
        margin-top: 2.875rem;
        width: 338.28px;
        height: 422px;
    }

    .logo_name {
        width: 15.724rem;
        height: 3.875rem;
    }

    .welcome-text__span {
        font-size: 1.75em;
    }

    .desc-text__desc {
        font-size: 1.125em;
        line-height: 1.625em;
        text-align: center;
        height: 4.875rem;
    }
}
</style>