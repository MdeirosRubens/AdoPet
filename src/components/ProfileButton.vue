<template>
    <div class="profilebutton">
        <a href="#">
            <img class="profilebutton__img" src="@/assets/imgs/icons/profile.svg" alt="Icone para tela de Perfil">
        </a>
    </div>

</template>

<script lang="ts">
import { defineComponent } from "vue"

export default defineComponent({
    name: 'ProfileButton'
})
</script>

<style>
.profilebutton {
    width: 2.5rem;
    height: 2.5rem;

}

.profilebutton__img {
    width: 2.5rem;
    height: 2.5rem;
}
</style>