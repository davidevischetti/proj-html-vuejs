<template>
<header class="container">

<div>
  <font-awesome-icon icon="fa-solid fa-clock"/>
  <span>Open Hours&colon; Mon &hyphen; Sat &hyphen; 9&colon;00 &hyphen; 18&colon;00 </span>
</div>

<div class="info">
  <a href="#">
    <font-awesome-icon icon="fa-solid fa-phone"/>
    <span>&plus;1 &lpar;305&rpar; 1234&hyphen;5678</span>
  </a>
  <a href="#">
    <font-awesome-icon icon="fa-solid fa-envelope"/>
    <span>hello&commat;example&period;com</span>
  </a>
    <a href="#"><font-awesome-icon icon="fa-brands fa-facebook-f"/></a>
    <a href="#"><font-awesome-icon icon="fa-brands fa-twitter"/></a>
    <a href="#"><font-awesome-icon icon="fa-brands fa-linkedin-in"/></a>
</div>

</header>
</template>

<script>
export default {
  name: 'MyHeader',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  width: 100%;
  height: 30px;
  background-color: #21333e;
  color: #ccc;
  font-size: 10px;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 300;

  a {
    color: #ccc;
  }

  span {
    margin-left: 5px;
  }

  .info {
  width: 40%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  }
}
</style>
