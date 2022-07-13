<template>
<header class="headerview">
    <NavHome/>
</header>
</template>

<script lang="ts">

import { defineComponent } from "vue";
import NavHome from "@/components/NavHome.vue";

export default defineComponent({
    Name: "HeaderView",
    components: { NavHome }
})
</script>

<style>
.headerview {
    background-image: url(@/assets/imgs/background/Forma.png);
    background-repeat: no-repeat;
    width: 100%;
    height: 18.438rem;
}
</style>