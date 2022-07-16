<template>
<HeaderView/>
<ProfileComponent/>
<FooterView/>
</template>

<script lang="ts">
import { defineComponent } from "vue"
import HeaderView from "./HeaderView.vue"
import FooterView from '@/views/FooterView.vue'
import ProfileComponent from "@/components/ProfileComponent.vue"


export default defineComponent({
    name: "ProfileView",
    components: { HeaderView, FooterView, ProfileComponent }
})
</script>

<style>

</style>