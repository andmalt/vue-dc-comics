<template>
    <main>
        <BoxDc/>
    </main>
</template>

<script>
import DcCard from '../data/dc-comics.json';
import BoxDc from './Box.vue';

export default {
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
    padding: 3rem;
    background-color: $colorContent;
}
</style>