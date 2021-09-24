<template>
  <header>
      <div id="img-logo">
          <img src="../assets/img/dc-logo.png" alt="logo DC">
      </div>

      <nav id="nav-h">
          <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">Tv</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Collectibles</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">Fans</a></li>
              <li><a href="#">News</a></li>
              <li><a href="#">Shops</a></li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "../style/variables.scss";

header{
    display: flex;
    justify-content: space-evenly;
    align-items: center;
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
            border-bottom: 2px solid transparent;


            &:active{
                border-bottom: 2px solid $logoColor;
                
            }
            & a{
                text-decoration: none;
                color: $colorContent;
                text-transform: uppercase;
                font-weight: 600;
                font-size: 1rem;
                font-family: $navFont;

                &:hover{
                    color: $logoColor;
                }
                &:active{
                    color: $logoColor
                }
            }
        }
    }
}



</style>