<template>
<section>
    <!-- colore svg impostato per puntini neri -->
    <img class="bullets up" src="../assets/svg/svg-0.svg" alt="bullets">
    <img class="bullets down" src="../assets/svg/svg-0.svg" alt="bullets">

    <div class="sp-container">
        <h5>ABOUT THE NETWORK</h5>
        <h2><div class="special-text">The</div> Company</h2>
        <p>For 12 years have been poviding audit and warranty&comma; financial advice&comma; risk advice&comma; taxes and releted services to select clients&period;</p>
        <!-- Ho usato icone sostituive perche' qulle presenti in screen mancavano dal materiale fornito -->
        <div class="info-card">
            <img src="../assets/svg/svg-1.svg" alt="logo">
            <h3>Tradition</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>
        <div class="info-card">
            <img src="../assets/svg/svg-1.svg" alt="logo">
            <h3>Security</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>
        <div class="info-card">
            <img src="../assets/svg/svg-1.svg" alt="logo">
            <h3>Certificate</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>
        <div class="info-card">
            <img src="../assets/svg/svg-1.svg" alt="logo">
            <h3>Expertise</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>
        <button class="btn btn-hover">GET IN TOUCH</button>
        <button class="btn">READ MORE</button>
    </div>

    <img id="bg-img-company" src="../assets/img/about-4.jpg" alt="logo">


</section>
</template>

<script>
export default {
    name: "CompanySection",
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
    background-color: #111117;
    display: flex;
    position: relative;

    .bullets {
        height: 100px;
        width: 150px;
        position: absolute;

        &.up {
            top: 0;
            left: 50%;
            transform: translate(-50%, -27%);
        }

        &.down {
            bottom: 0;
            left: 50%;
            transform: translate(-50%, 70%);
        }
    }

    

    #bg-img-company {
        width: 50%;
        height: 700px;
        object-fit: cover;
    }
    

    .sp-container {   
        width: 50%;      

        h5 {
        color: #54b0c1;
        width: 100%;

        }

        h2 {
            font-size: 40px;
            width: 100%;
            color: #fff;

            .special-text {
                color: #fff;
                background-color: #0e272d;    
            }
        }  

        p {
            color: #aaa;
            font-size: 15px;
            margin-bottom: 40px;
            
        } 

        .info-card {
            flex-basis: 45%;
            display: flex;
            justify-content: flex-start;
            align-items: center;
            flex-wrap: wrap;
            margin-right: 20px;

            img {
                width: 15px;
                height: 15px;
                margin-right: 15px;
            }

            h3 {
                color: #fff;
            }

            p {
                margin-top: 15px;
            }

            
        }

        .btn-hover {
            margin-right: 20px;
        }

        .btn {
            color: #fff;
        }
    }

    
}
</style>
