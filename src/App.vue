<template>
  <div id="app">
    <MyHeader/>
    <MyJumbo/>
    <ServicesSection/>
    <CompanySection/>
    <ProjectsSection/>
    <ResultsSection/>
    <ContactSection/>
    <FooterSection/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyJumbo from './components/MyJumbo.vue'
import ServicesSection from './components/ServicesSection.vue'
import CompanySection from './components/CompanySection.vue'
import ProjectsSection from './components/ProjectsSection.vue'
import ResultsSection from './components/ResultsSection.vue'
import ContactSection from './components/ContactSection.vue'
import FooterSection from './components/FooterSection.vue'
import MyFooter from './components/MyFooter.vue'


export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbo,
    ServicesSection,
    CompanySection,
    ProjectsSection,
    ResultsSection,
    ContactSection,
    FooterSection,
    MyFooter
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

  .sp-container {
        flex-wrap: wrap;
        padding:80px 20%;
        padding-right: 20px;
        display: flex;
        justify-content: flex-start;
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
    color: #038484;

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
