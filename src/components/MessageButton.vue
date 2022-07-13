<template>
    <div class="messagebutton">
        <a href="#">
            <img class="messagebutton__img" src="@/assets/imgs/icons/message.svg" alt="Icone para tela de mensagens">
        </a>
    </div>
</template>

<script lang="ts">
import { defineComponent } from "vue"

export default defineComponent({
    name: 'MessageButton'
})
</script>

<style>
.messagebutton {
    width: 2.5rem;
    height: 2.5rem;
    display: flex;
    align-items: center;
}

.messagebutton__img {
    width: 1.446rem;
    height: 1.179rem;
}
</style>