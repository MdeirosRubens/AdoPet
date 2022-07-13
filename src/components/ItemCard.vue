<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "ItemCard"
})

</script>

<style>
.card {
    width: 100%;
    height: 12.063rem;
    background-color: #F7F7F7;
    display: flex;
    justify-content: space-evenly;
    font-family: 'Poppins';
    margin-bottom: 1.25rem;
}

.card__picture {
    display: flex;
    align-items: center;
}

.card__infos {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}

.name {
    font-weight: 600;
    color: #3772FF;
    line-height: 1.25em;

}

.about {
    font-size: 0.875em;
    color: #737380;
    line-height: 1.25em;
}

.about p {
    padding: 0.125rem;
}

.info {
    color: #737380;
    line-height: 1.25em;
}

.info__adress {
    font-size: 0.75em;
    margin-bottom: 0.313rem;
}

.info__link {
    font-size: 0.625em;
    display: flex;
}

.info__link p {
    padding-left: 0.625rem;
}
</style>