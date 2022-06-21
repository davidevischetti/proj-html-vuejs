<template>
<div id="project-card">  
    <div>
        <a href="#"><font-awesome-icon icon="fa-solid fa-arrow-right"/></a>
        <h3>{{addProject.text}}</h3>
        <p>{{addProject.info}}</p>
    </div>
    <img :src="addProject.img" alt="img">  
</div>

</template>

<script>
export default {
    name: "ProjectsCard",
    props : ['addProject']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#project-card {
    width: 280px;
    height: 280px;
    margin-bottom: 25px;
    border-radius: 10px;
    position: relative;

    &:hover img {
            filter: blur(2px);
            transition: all 0.5s;
        }

    img {
        width: 100%;
        border-radius: 10px;
    }

    div {
        width: 100%;
        height: 100%;
        z-index: 30;
        position: absolute;
        top: 0;
        left: 0;
        padding: 20px 0;
        display: flex;
        flex-flow: column wrap;
        justify-content: flex-end;
        background-color: rgba(50, 50, 50, 0.5);
        cursor: pointer;

        &:hover p,
        &:hover a { 
            display: block;
        }
        
        h3 {
            color: #fff;
            text-align: center;
            margin-bottom: 15px;
        }

        p {
            color: #ddd;
            font-size: 15px;
            text-align: center;
            padding: 10px 30px;
            display: none;
            font-weight: 600;  
        }

        a {
            font-size: 20px;
            color: #fff;
            position: absolute;
            top: 20px;
            right: 20px;
            display: none;
        }
    }

}
</style>
