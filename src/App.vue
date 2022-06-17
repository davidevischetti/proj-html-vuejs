<template>
  <div id="app">
    <MyHeader/>
    <MyJumbo/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyJumbo from './components/MyJumbo.vue'


export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbo
}
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Arial, Helvetica, sans-serif;

  .container {
    padding: 0 20%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  ul {
    list-style-type: none;
  }

  a {
    text-decoration: none;
  }

  .btn {
    padding: 10px 20px;
    color: #fff;
    background-color: #038484;
    border: none;
    border-radius: 3px;
  }
}
</style>
