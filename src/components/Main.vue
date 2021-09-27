<template>
    <main>
        <BoxDc v-for="(element, index ) in DcCard" :key="index" :series="element.series" :thumb="element.thumb" />
        <div class="btn-main">
            <button>LOAD MORE</button>
        </div>
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
    padding: 3rem 10rem 1rem;
    background-color: $colorContent;
    & .btn-main{
        margin: 1rem 0 0.5rem;
    }
    & button{
        background-color: $logoColor;
        border: 2px solid $logoColor;
        padding: 0.5rem 2rem;
        color: $fontMain;
        font-size: 0.8rem;
        font-weight: 600;
    }
}
</style>