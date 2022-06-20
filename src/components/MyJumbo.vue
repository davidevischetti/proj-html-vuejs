<template>
<section>
  <div id="hero">
    <MyNavBar/>

    <div id="hero-text">
      <h1>READY<div class="special-text">TEAM</div></h1>
      <p>No matter what your company needs, we will be ready to assist you in the best possible way.</p>
      <div>
        <button class="btn btn-hover">GET IN TOUCH</button>
        <button class="btn">READ MORE</button>
      </div>
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
section {
  background-image: url(https://img.freepik.com/free-vector/abstract-technology-white-gray-color-modern-background_41981-1010.jpg?w=2000);
  background-size: cover;
}
#hero {
  background-image: url(../assets/img/bg-parallax.png);
  background-size: 190% ;
  background-position: center;
  background-repeat: no-repeat;
  width: 100%;
  height: 90vh;
  margin-top: 30px;

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

    .btn:hover {
      color: #fff;
      background-color: #038484;
    }

  }
}
</style>
