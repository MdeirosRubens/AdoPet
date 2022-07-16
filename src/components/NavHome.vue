<template>
    <nav class="nav">
        <div class="separatedicon">
            <HomeButton />
            <MessageButton />
        </div>
    </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HomeButton from "./HomeButton.vue";
import MessageButton from "./MessageButton.vue";


export default defineComponent({
    name: "NavApp",
    components: { HomeButton, MessageButton }
})
</script>

<style>
.nav {
    display: flex;
    justify-content: space-between;
    padding: 2rem;
}

.separatedicon{
    width: 50%;
    display: flex;
    justify-content: space-around;
}

@media (min-width: 1140px) {
    .separatedicon {
        width: 30%;
    }
}
</style>