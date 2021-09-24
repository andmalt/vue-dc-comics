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
        & li{
            padding: 0 1rem 0;
            & a{
                text-decoration: none;
                color: $colorContent;
            }
        }
    }
}



</style>