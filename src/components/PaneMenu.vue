<template>
    <div id="pane-menu">
        <ul>
            <li><a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt="logo DC">DIGITAL COMICS</a></li>
            <li><a href="#"><img src="../assets/img/buy-comics-merchandise.png" alt="logo merchandise">DC MERCHANDISE</a></li>
            <li><a href="#"><img src="../assets/img/buy-comics-subscriptions.png" alt="logo subscription">SUBSCRIPTIONS</a></li>
            <li><a href="#"><img src="../assets/img/buy-comics-shop-locator.png" alt="logo shop locator">COMIC SHOP LOCATOR</a></li>
            <li><a href="#"><img src="../assets/img/buy-dc-power-visa.svg" alt="logo PW">DC POWER VISA</a></li>
        </ul>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "../style/variables.scss";
#pane-menu{
    background-color: $logoColor;
    height: 150px;
    text-align: center;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    & ul{
        display: flex;
        flex-wrap: wrap;
        & li{
        list-style: none;
        margin: 0.5rem 1rem;
        & a{
            color: $fontMain;
            text-decoration: none;
            font-size: 0.9rem;
        }
        & img{
            height: 35px;
            margin-right: 8px;
        }
    }
    }
    
}
</style>