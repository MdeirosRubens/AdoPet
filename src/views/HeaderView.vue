<template>
<header class="headerview">
    <NavApp/>
</header>
</template>

<script lang="ts">

import { defineComponent } from "vue";
import NavApp from "@/components/NavApp.vue";

export default defineComponent({
    Name: "HeaderView",
    components: { NavApp }
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