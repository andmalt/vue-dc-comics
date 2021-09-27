<template>
        <div class="box-dc">
            <img :src="thumb" :alt="series">
            <h6>{{ series }}</h6>
        </div>
</template>

<script>
export default {
    name:'Box',
    props:{
        thumb:String,
        price:String,
        series:String,
        types:String,
    }   
}
</script>

<style lang='scss'>
@import "../style/variables.scss";
.box-dc{
    flex-basis: calc(100% / 6 - 8px);
    height: 280px;
    margin: 4px;
    text-align: center;
    & img{
        height: 85%;
    }
    & h6{
        font-size: 1rem;
        font-weight: 600;
        color: $fontMain;
        font-family: $navFont;
    }
}
</style>