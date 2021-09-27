<template>
    <main>
        <BoxDc v-for="(element, index ) in DcCard" :key="index" :series="element.series" :thumb="element.thumb" />
    </main>
</template>

<script>
import DcCard from '../data/dc-comics.json';
import BoxDc from './Box.vue';

export default {
    name:'Main',
    components: {
        BoxDc,
    },
    data: function(){
        return{
            DcCard,
        }
    }
}
</script>

<style lang="scss">
@import "../style/variables.scss";

main{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    padding: 3rem 10rem;
    background-color: $colorContent;
}
</style>