<template>
  <header>
      <div id="img-logo">
          <img src="../assets/img/dc-logo.png" alt="logo DC">
      </div>

      <nav id="nav-h">
          <ul>
              <li v-for="(element, index) in links" :key="index" :class="{ active : element.current}"> 
                  <a> {{ element.text }} </a>
              </li>
          </ul>
      </nav>
      
  </header>
</template>

<script>
export default {
    name: 'Header',
    data: function () {
    return {
      links:[
        {
            text: "Characters",
            url:'#characters',
            current: true,
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
            text: "Collectibles",
            url:'#collectibles',
            current: false,
        },
                {
            text: "Videos",
            url:'#videos',
            current: false,
        },
        {
            text: "Fans",
            url:'#fans',
            current: false,
        },
                {
            text: "News",
            url:'#news',
            current: false,
        },
        {
            text: "Shops",
            url:'#shops',
            current: false,
        },
      ]
    }
  },
}
</script>

<style lang="scss">
@import "../style/variables.scss";

header{
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    position: relative;
    z-index: 3;
}

#img-logo{
    width: 60px;
    & img{
        width: 100%;
    }
}
#nav-h{
    text-align: center;
    & ul{
        list-style: none;
        display: flex;
        padding: 0;
        & li{
            padding: 2.5rem 1rem;
            border-bottom: 4px solid transparent;

            &.active{
                border-bottom: 4px solid $logoColor;
                
            }


            & a{
                text-decoration: none;
                color: $colorContent;
                text-transform: uppercase;
                font-weight: 600;
                font-size: 1rem;
                font-family: $navFont;
                z-index: 5;

                &:hover{
                    color: $logoColor;
                }
            }
        }
    }
}



</style>