<template>
  <div id="app">
    <MyHeader/>
    <MyJumbo/>
    <ServicesSection/>
    <CompanySection/>
    <ProjectsSection/>
    <ResultsSection/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyJumbo from './components/MyJumbo.vue'
import ServicesSection from './components/ServicesSection.vue'
import CompanySection from './components/CompanySection.vue'
import ProjectsSection from './components/ProjectsSection.vue'
import ResultsSection from './components/ResultsSection.vue'


export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbo,
    ServicesSection,
    CompanySection,
    ProjectsSection,
    ResultsSection
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
    background-color: transparent;
    border: 1px solid #038484;
    border-radius: 5px;
    cursor: pointer;

    &:hover {
        color: #fff;
        background-color: #038484;
        transform: scale(110%);
        transition: all 0.5s;
    }
  }

  .btn-hover {
    color: #fff;
    background-color: #038484;
  }

  .special-text {
    display: inline-block;
    padding: 5px 20px;
    border-radius: 5px;
  }

}
</style>
