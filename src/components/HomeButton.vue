<template>
    <div class="homebutton">
        <a href="#">
            <img class="homebutton__img" src="@/assets/imgs/icons/home.svg" alt="Icone para página inicial">
        </a>
    </div>
</template>

<script lang="ts">
import { defineComponent } from "vue"

export default defineComponent({
    name: 'HomeButton'
})
</script>

<style>
.homebutton {
    width: 2.5rem;
    height: 2.5rem;
    display: flex;
    align-items: center;
}

.homebutton__img {
    width: 1.438rem;
    height: 1.438rem;
}
</style>