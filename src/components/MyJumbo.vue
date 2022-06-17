<template>
<section id="hero">
  <MyNavBar/>
</section>
</template>

<script>
import MyNavBar from './MyNavBar.vue';
export default {
    name: "MyJumbo",
    components: { MyNavBar }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#hero {
  background-image: url(../assets/img/bg-parallax.png);
  background-size: 200% ;
  background-position: center;
  background-repeat: no-repeat;
  width: 100%;
  height: 90vh;
  margin-top: 50px;
}
</style>
