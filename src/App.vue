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
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

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
    padding: 8px 20px;
    color: #038484;
    background-color: transparent;
    border: 1px solid #038484;
    border-radius: 5px;
  }

  .btn-hover {
    color: #fff;
    background-color: #038484;
    border: none;
  }

}
</style>
