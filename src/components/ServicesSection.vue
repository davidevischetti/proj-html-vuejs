<template>
<section>
<div class="container">
  <h5>OUR BUSINESS AREAS</h5>
  <h2>Exellence in<div class="special-text">Services</div></h2>
  <p>We are leaders in providing consultanc with a set of cutting&hyphen;edge technologies and a team of experienced and renowned professionals&period; These are some options that you can hire&period;</p>
  <button class="btn btn-hover">SEE ALL</button>
</div>

<div class="container">
  <ServicesCard v-for="(service, i) in servicesList" :key="i" :addService="service" />
  
</div>

</section>
</template>

<script>
import ServicesCard from './ServicesCard.vue';
export default {
    name: "ServicesSection",
    components: { ServicesCard },
    data () {
      return {
        servicesList : [
          {
            img:require('../assets/svg/svg-1.svg'),
            text:'Audit & Assurance',
            info:'Audit & Assurance Audit & Assurance Audit & Assurance Audit & Assurance',
          },
          {
            img:require('../assets/svg/svg-2.svg'),
            text:'Financial Advisory',
            info:'Financial Advisory Financial Advisory Financial Advisory Financial Advisory',
          },
          {
            img:require('../assets/svg/svg-3.svg'),
            text:'Analytics and M&a',
            info:'Analytics and M&a Analytics and M&a Analytics and M&a Analytics and M&a',
          },
          {
            img:require('../assets/svg/svg-4.svg'),
            text:'Middle Marketing',
            info:'Middle Marketing Middle Marketing Middle Marketing Middle Marketing',
          },
          {
            img:require('../assets/svg/svg-5.svg'),
            text:'Legal Consulting',
            info:'Legal Consulting Legal Consulting Legal Consulting Legal Consulting',
          },
          {
            img:require('../assets/svg/svg-6.svg'),
            text:'Regulatory Risk',
            info:'Regulatory Risk Regulatory Risk Regulatory Risk Regulatory Risk',
          },
        ]
      }
    }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
  padding: 80px 0;
  background-color: #eef4ed;

  .container {
    flex-wrap: wrap;
    margin-bottom: 20px;

    h5 {
      color: #54b0c1;
      width: 100%;
    }

    h2 {
      font-size: 40px;
      width: 100%;
      margin: 20px 0;
    }

    p {
      color: #666;
      font-size: 15px;
      width: 70%;
    }
  }

}
</style>
