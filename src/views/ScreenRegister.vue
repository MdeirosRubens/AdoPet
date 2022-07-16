<template>
    <div class="header-cadastro">
        <HeaderView />
    </div>
    <img class="patas-icon" src="@/assets/imgs/patas.png" alt="Ilustração de Patas" />
    <section class="container-cadastro">
        <div class="logo">
            <img src="@/assets/imgs/logos/logo_azul.svg" alt="">
        </div>
        <div class="desc-text">
            <span class='quest-text__span'>Ainda não tem cadastro?</span>
        </div>
        <div class="desc-text">
            <p class="desc-text__desc">
                Então, antes de buscar seu melhor amigo, precisamos de alguns dados:
            </p>
        </div>
    </section>
    <section class="formulario-section">
        <form class="form" action="">
            <div class="input-container">
                <label for="input-label">Email</label>
                <input class="input" type="email" placeholder="Escolha seu melhor email">
            </div>
            <div class="input-container">
                <label for="input-label">Nome</label>
                <input class="input" type="text" placeholder="Digite seu nome completo">
            </div>
            <div class="input-container">
                <label for="input-label">Senha</label>
                <input class="input" type="password" placeholder="Crie uma senha">
            </div>
            <div class="input-container">
                <label for="input-label">Confirme sua senha</label>
                <input class="input" type="password" placeholder="Repita a senha criada acime">
            </div>
            <div class="form-button">
                <button class="btn-small">Cadastrar</button>
            </div>
        </form>
    </section>
    <FooterView/>

</template>

<script lang="ts">

import { defineComponent } from "vue";
import HeaderView from "./HeaderView.vue";
import FooterView from "./FooterView.vue";

export default defineComponent({
    name: "TelaCadastro",
    components: { HeaderView, FooterView }
})

</script>

<style>

.profilebutton {
  display: none;
}

.patas-icon {
    z-index: 10;
    position: fixed;
    top: 0%;
    right: 0%;
}

.container-cadastro {
    font-family: 'Poppins', sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
    position: absolute;
    top: 20%;
}

.desc-text {
    color: #3772FF;
}

.quest-text__span {
    font-weight: 500;
    line-height: 3em;
}

.desc-text__desc {
    font-weight: 400;
    line-height: 1.5em;
    text-align: center;
    height: 4.5rem;
}

.formulario-section {
    display: flex;
    flex-direction: column;   
}

.form {
    background-image: url(@/assets/imgs/background/Forma_3.png);
    background-repeat: no-repeat;
    margin-top: 2.5rem;
}

.input-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    font-family: 'Poppins';
    font-style: normal;
    line-height: 2.75em;
    margin-bottom: 0.625rem;
}

.input-label {
    color: #737380;
}

.input {
    width: 19.5rem;
    height: 2.5rem;
    background-color: #F6F6F6;
    border: none;
    box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.15);
    border-radius: 6px;
    font-family: 'Poppins';
    text-align: center;
}
</style>