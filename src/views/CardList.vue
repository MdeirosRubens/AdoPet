<template>
    <HeaderView />
    <section class="text__span">
        <span>Olá! Veja os amigos disponíveis para adoção!</span>
    </section>
    <section>
        <ItemCard/>
        <ItemCard/>
        <ItemCard/>
        <ItemCard/>
        <ItemCard/>
        <ItemCard/>
    </section>
    <FooterView />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HeaderView from "./HeaderView.vue";
import FooterView from "./FooterView.vue";
import ItemCard from "@/components/ItemCard.vue";

export default defineComponent({
    name: "CardList",
    components: { HeaderView, FooterView, ItemCard }
})

</script>

<style>
.text__span {
    color: #3772FF;
    line-height: 1.25em;
    font-family: 'Poppins';
    text-align: center;
    top: 20%;
    width: 16rem;
    position:fixed;
    left: 17%;
    display: flex;
    z-index: -1;
}

.text__span span {
    font-size: 1em;
}
</style>