<template>
  <div id="app">
    <MyHeader/>
    <MyJumbo/>
    <ServicesSection/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyJumbo from './components/MyJumbo.vue'
import ServicesSection from './components/ServicesSection.vue'


export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbo,
    ServicesSection
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
    cursor: pointer;
  }

  .btn-hover {
    color: #fff;
    background-color: #038484;

  }

  .special-text {
  display: inline-block;
  color: #058283;
  background-color: #d5e7e8;
  padding: 0 20px;
  border-radius: 5px;
  margin-left: 10px;
  }

}
</style>
