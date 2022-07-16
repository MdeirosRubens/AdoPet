<template>
    <nav class="nav">
        <div class="separatedicon">
            <img class="logo-on-media" src="@/assets/imgs/logos/logo_branco.svg" alt="Logo da AdoPet">
            <HomeButton />
            <MessageButton />
        </div>
        <ProfileButton />
    </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HomeButton from "./HomeButton.vue";
import MessageButton from "./MessageButton.vue";
import ProfileButton from "./ProfileButton.vue";

export default defineComponent({
    name: "NavApp",
    components: { HomeButton, MessageButton, ProfileButton }
})
</script>

<style>
.logo-on-media {
    display: none;
}

.nav {
    display: flex;
    justify-content: space-between;
    padding: 2rem;
}

.separatedicon {
    width: 50%;
    display: flex;
    justify-content: space-around;
}

@media (min-width: 768px) {
    .logo-on-media {
        display: block;
        width: 8rem;
    }
}

@media (min-width: 1140px) {
    .separatedicon {
        width: 30%;
    }
}
</style>