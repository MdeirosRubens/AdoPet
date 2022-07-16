<template>
<footer class="footer">
    <span class="footer__text">2022 - Desenvolvido por Rubens Medeiros.</span>
</footer>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: 'FooterView'
})
</script>

<style>
.footer {
    height: 7rem;
    width: 100%;
    background-color: #36D6AD;
    display: flex;
    align-items: center;
    justify-content: center;
}

.footer__text {
    color: #fff;
    font-family: 'Poppins', sans-serif;
}
</style>