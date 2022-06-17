<template>
<nav class="container">
<img src="../assets/svg/svg-7.svg" alt="logo">

<div id="nav-bar">
    <ul>
        <li v-for="(link,i) in headerLinks" :key="i">
            <a href="#">{{link}}</a>
        </li>
    </ul>
    <button class="btn">GET IN TOUCH</button>
</div>

</nav>
</template>

<script>
export default {
    name: "MyNavBar",
    data () {
        return {
            headerLinks : ['HOME', 'SERVICES', 'ABOUT', 'PROJECT', 'RESULTS']
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
nav {
    height: 50px;
    width: 100%;

    img {
        height: 80%;
    }

    #nav-bar {
        display: flex;
        align-items: center;
        ul {
            li {
                display: inline-block;
                margin-right: 20px;
                
                a {
                    color: #777;
                    font-size: 15px;
                    font-weight: 600;
                }
            }
        }
    }

}
</style>
