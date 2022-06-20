<template>
<div id="service-card">
    <img :src="addService.img" alt="img">
    <a href="#"><font-awesome-icon icon="fa-solid fa-arrow-right"/></a>
    <h3>{{addService.text}}</h3>
    <p>{{addService.info}}</p>
</div>
</template>

<script>
export default {
    name: "ServicesCard",
    props : ['addService']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#service-card {
    padding: 30px;
    flex-basis: 30%;
    background-color: #fff;
    border-radius: 10px;
    margin-top: 20px;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;

    
    img {
        width: 30px;
        height: 30px;
    }

    a {
        color: #54b0c1;
    }

    h3 {
        width: 100%;
        margin: 20px 0;
    }

    p {
        font-size: 12px;
        color: #666;
        margin-bottom: 10px;
    }

}
</style>
