<template>
<section id="hero">
  <MyNavBar/>

  <div id="hero-text">
    <h1>READY<div>TEAM</div></h1>
    <p>No matter what your company needs, we will be ready to assist you in the best possible way.</p>
    <div>
      <button class="btn btn-hover">GET IN TOUCH</button>
      <button class="btn">READ MORE</button>
    </div>
  </div>
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

  #hero-text {
    height: calc(100% - 50px);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    h1 {
      font-size: 60px;
      font-weight: 900;
      margin-bottom: 30px;

      div {
        display: inline-block;
        color: #058283;
        background-color: #d5e7e8;
        padding: 0 20px;
        border-radius: 5px;
        margin-left: 10px;
       }
    }

    p {
      width: 25%;
      text-align: center;
      color: #888;
      margin-bottom: 40px;
    }

    .btn-hover {
      margin-right: 20px;
    }

  }
}
</style>
