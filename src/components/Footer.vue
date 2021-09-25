<template>
    <footer>
        <div id="main-footer">
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
        </div>
            

        <div id="footer-bottom">
            <div class="btn-footer">
                <button>SIGN-UP NOW!</button>
            </div>

            <div class="social">
                <h3>FOLLOW US</h3>
                <ul>
                    <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="logo facebook"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="logo twitter"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="logo youtube"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="logo pinterest"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="logo periscope"></a></li>
                </ul>
            </div>
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
    flex-direction: column;
}
.columns{
    margin: 0 0.7rem;
}
.btn-footer{
    text-align: center;
    display: inline-block;
    
    & button{
        background-color: $footerBottom;
        padding: 0.7rem;
        color: white;
        border: 2px solid $logoColor;
        font-weight: 600;
        &:hover{
            background-color: $logoColor;
        }
    }
}
.social{
    display: inline-block;
    display: flex;
    justify-content: center;
    align-items: center;
    & h3{
        color: $logoColor;
        margin-right: 1rem;
    }
    & ul {
        display: flex;
        justify-content: space-between;
        list-style: none;
        & li {
            margin: 0.5rem;
        };
    }
}
#main-footer{
    display: flex;
    justify-content: space-around;
    align-items: center;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position-y: top;
    z-index: -5;
    font-family: $navFont;
    padding: 3rem;
}

#navs-f{
    display: flex;
    justify-content: space-around;
    & h4{
        color: $fontFooter;
        padding: 0.5rem 0;
        font-size: 1.4rem;
        font-weight: 600;
    }
    & ul li{
        list-style: none;
        padding: 0.2rem 0;
        z-index: 5;
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
    & img{
        width: 100%;
    }
}
#footer-bottom{
    background-color: $footerBottom;
    padding: 2rem;
    width: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
}
</style>