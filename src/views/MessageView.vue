<template>
<HeaderView/>
<FormComponent/>
<FooterView/>
</template>

<script lang="ts">
import { defineComponent } from "vue"
import FormComponent from "@/components/FormComponent.vue"
import HeaderView from "./HeaderView.vue"
import FooterView from '@/views/FooterView.vue'


export default defineComponent({
    name: "MessageView",
    components: { FormComponent, HeaderView, FooterView }
})
</script>

<style>

</style>