<template>
    <footer>
        <div id="navs-f">
            <div class="columns">
                <h4>Dc Comics</h4>
                <ul>
                    <li v-for="(element, index) in linkFooter" :key="index"> 
                        <a> {{ element.text }} </a>
                    </li>
                </ul>
                

                <h4>Shops</h4>
                <ul>
                    <li v-for="(element, index) in linkShop" :key="index"> 
                        <a> {{ element.text }} </a>
                    </li>
                </ul>
                

            </div>
                
            <div class="columns">
                <h4>Dc</h4>
                <ul>
                    <li v-for="(element, index) in linkDc" :key="index"> 
                        <a> {{ element.text }} </a>
                    </li>
                </ul>
                
            </div>

            <div class="columns">
                <h4>Sites</h4>
                <ul>
                    <li v-for="(element, index) in linkSites" :key="index"> 
                        <a> {{ element.text }} </a>
                    </li>
                </ul>
            </div>
        </div>
        
        <div id="img-bg-f">
            <img src="../assets/img/dc-logo-bg.png" alt="logo DC">
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    data: function () {
    return {
        linkFooter:[
            {
                text: "Characters",
                url:'#characters',
                current: false,
            },
            {
                text: "Comics",
                url:'#comics',
                current: false,
            },
                    {
                text: "Movies",
                url:'#movies',
                current: false,
            },
            {
                text: "Tv",
                url:'#tv',
                current: false,
            },
                    {
                text: "Games",
                url:'#games',
                current: false,
            },
            {
                text: "Videos",
                url:'#videos',
                current: false,
            },
            {
                text: "News",
                url:'#news',
                current: false,
            },
        ],
        linkShop:[
          {
                text: "Shop DC",
                url:'#shopDc',
                current: false,
            },
            {
                text: "Shop DC Collectibles",
                url:'#shopDcCollectibles',
                current: false,
            },  
        ],
        linkDc:[
            {
                text: "Terms Of Use",
                url:'#termsOfUse',
                current: false,
            },
            {
                text: "Privacy policy (New)",
                url:'#privacyPolicy',
                current: false,
            },
            {
                text: "Ad Choises",
                url:'#adChoises',
                current: false,
            },
            {
                text: "Advertising",
                url:'#advertising',
                current: false,
            },
                    {
                text: "Jobs",
                url:'#jobs',
                current: false,
            },
            {
                text: "Subscriptions",
                url:'#subscriptions',
                current: false,
            },
            {
                text: "Talent Workshops",
                url:'#talentWorkshops',
                current: false,
            },
             {
                text: "CPSC Certificates",
                url:'#CPSCcertificates',
                current: false,
            },
                    {
                text: "Ratings",
                url:'#ratings',
                current: false,
            },
            {
                text: "Shop help",
                url:'#shopHelp',
                current: false,
            },
            {
                text: "Contact Us",
                url:'#contactUs',
                current: false,
            },
        ],
        linkSites:[
            {
                text: "DC",
                url:'#dc',
                current: false,
            },
            {
                text: "MAD Magazine",
                url:'#MADmagazine',
                current: false,
            },
            {
                text: "DC Kids",
                url:'#DCkids',
                current: false,
            },
            {
                text: "DC Universe",
                url:'#DCuniverse',
                current: false,
            },
            {
                text: "DC Power Visa",
                url:'#DCpowerVisa',
                current: false,
            },
        ],
    }
  },
}
</script>

<style lang="scss">
@import "../style/variables.scss";
footer{
    display: flex;
    justify-content: space-around;
    align-items: center;
    background-image: url(../assets/img/footer-bg.jpg);
    background-position: center;
    z-index: -5;
    font-family: $navFont;
}
.columns{
    margin: 0 0.7rem;
}
#navs-f{
    display: flex;
    justify-content: space-around;
    & h4{
        color: $fontFooter;
        padding: 0.5rem 0;
        font-size: 1.3rem;
        font-weight: 600;
    }
    & ul li{
        list-style: none;
        padding: 0.2rem 0;
        & a{
            color: rgb(145, 145, 145);
            font-size: 1rem;
            text-decoration: none;
        }
    }
}
#img-bg-f{
    width: 250px;
    transform: scale(2);
    z-index: 1;
    & img{
        width: 100%;
    }
}
</style>