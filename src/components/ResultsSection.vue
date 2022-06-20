<template>
<section>
    <div id="results-numbers" class="container">
        <div>
            <h5>WHATARE WE DOING</h5>
            <h2><div class="special-text">Results</div> in Numbers</h2>
        </div>
        <div class="numbers">
            <div v-for="(number, i) in numbersList" :key="i">
                <h3>{{number.num}}</h3>
                <span>{{number.text}}</span>
            </div>
        </div>
    </div>
    <div id="partners-list" class="container">
        <div v-for="(partner, index) in partnersList" :key="index" >
            <img :src="partner.img" :alt="partner.text">
        </div>
    </div>

</section>
</template>

<script>
export default {
  name: 'ResultsSection',
  data () {
    return {
        numbersList : [
            {
                num : '128',
                text : 'Certifications'
            },
            {
                num : '230',
                text : 'Employees'
            },
            {
                num : '517',
                text : 'Customers'
            },
            {
                num : '94',
                text : 'Countries Served'
            }
        ],

        partnersList : [
            {
                text: 'jQuery',
                img: require('../assets/img/logo-4.png')
            },
            {
                text: '{less}',
                img: require('../assets/img/logo-5.png')
            },
            {
                text: 'WooCommerce',
                img: require('../assets/img/logo-1.png')
            },
            {
                text: 'WordPress',
                img: require('../assets/img/logo-2.png')
            },
            {
                text: 'pingdom',
                img: require('../assets/img/logo-3.png')
            },
            {
                text: 'jQuery',
                img: require('../assets/img/logo-4.png')
            },
        ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
    background-color: #111117;

    #results-numbers {
        width: 100%;
        background-image: url(../assets/img/bg-7.jpg);
        background-size: cover;
        background-position: center;
        flex-direction: column;

        h5 {
            color: #54b0c1;
            width: 100%;
            text-align: center;
            margin-top: 80px;
        }

        h2 {
            font-size: 40px;
            width: 100%;
            color: #fff;
            margin: 30px 0;

            .special-text {
                color: #fff;
                background-color: #0e272d;    
            }
        } 

        .numbers {
            display: flex;
            justify-content: space-around;
            align-items: center;
            width: 100%;
            margin-top: 50px;
            margin-bottom: 120px;

            h3 {
                font-size: 30px;
                color: #00a6a6;
                text-align: center;
                margin: 10px;
            }

            span {
                color: #fff;
                font-weight: 600;
            }
        }
    }

    #partners-list {
        div {
            margin: 80px 0;

            img {
                height: 22px;
                filter: invert(50%);
            }
        }
    }    
}   
</style>
