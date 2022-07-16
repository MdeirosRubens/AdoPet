<template>
    <div class="text__span">
        <p>
            Envie uma mensagem para a pessoa ou instituição que está cuidado do animal:
        </p>
    </div>
    <div class="form-container">
        <form action="" class="form">
            <div class="input-container">
                <label for="input-label">Nome</label>
                <input class="input" type="text" placeholder="Insira seu nome completo">
            </div>
            <div class="input-container">
                <label for="input-label">Telefone</label>
                <input class="input" type="tel" placeholder="Insira seu telefone e/ou whatsapp">
            </div>
            <div class="input-container">
                <label for="input-label">Nome do animal</label>
                <input class="input" type="text" placeholder="Por qual animal você se interessou?">
            </div>
            <div class="input-container">
                <label for="input-label">Mensagem</label>
                <textarea class="textarea" placeholder="Escreva sua mensagem"></textarea>
            </div>
            <div class="form-button">
                <button class="btn-small">Enviar</button>
            </div>
        </form>
    </div>
</template>

<script lang="ts">
import { defineComponent } from "vue"


export default defineComponent({
    name: "FormComponent",
    components: {

    }
})
</script>

<style>
.form-container {
    display: flex;
    justify-content: center;
    margin-bottom: 10px;
}

.form {
    display: flex;
    flex-direction: column;
    width: 88%;
    padding: 2%;
    background-color: #f6f6f6;
    border-radius: 10px;
    color: #3772FF;
}

.input-container {
    display: flex;
    flex-direction: column;
    font-family: 'Poppins';
    line-height: 2.75em;
    margin-bottom: 0.625rem;
    font-weight: 600;
}

.input {
    width: 18.9rem;
    height: 2.5rem;
    border: none;
    box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.15);
    border-radius: 6px;
    font-family: 'Poppins';
    font-size: 0.875em;
    padding: 0 0 0 0.938rem;
}

.textarea {
    height: 10.75rem;
    border: none;
    box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.15);
    border-radius: 6px;
    font-family: 'Poppins';
    font-size: 0.875em;
    padding: 0.938rem 0 0 0.938rem;
}
</style>