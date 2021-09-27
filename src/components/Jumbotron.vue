<template>
  <section id="jumbotron">
      <div>
          <h1>Jumbotron</h1>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang='scss'>
#jumbotron{
    background-color: gray;
    width: 100%;
    height: 300px;
    text-align: center;
    & h1{
        padding: 3rem;
    }
}
</style>