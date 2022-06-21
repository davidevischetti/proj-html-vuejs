<template>
<nav class="container">
    <!-- Immagine logo navbar sostituita con logo footer causa errore di caricamento-->
<img src="../assets/svg/svg-7.svg" alt="logo">

<div id="nav-bar">
    <ul>
        <li v-for="(link,i) in headerLinks" @click="activeLinkFunc(link)" :key="i" :class="link.active ? 'select' : ''">
            <a href="#">{{link.text}}</a>
        </li>
    </ul>
    <button class=" btn btn-hover">GET IN TOUCH</button>
</div>
</nav>


</template>

<script>
export default {
    name: "MyNavBar",
    data () {
        return {
            headerLinks : [
                {
                    text : 'HOME',
                    active : true
                },
                {
                    text : 'SERVICES',
                    active : false
                },
                {
                    text : 'ABOUT',
                    active : false
                },
                {
                    text : 'PROJECT',
                    active : false
                },
                {
                    text : 'RESULTS',
                    active : false
                }
            ]
        }
    },
    methods : {
        activeLinkFunc (activeLink) {
            this.headerLinks.forEach(element => {
            element.active = false
            });

            activeLink.active = true
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
        margin-top: 20px;
    }

    #nav-bar {
        display: flex;
        align-items: center;
        margin-top: 20px;
        ul {
            li {
                display: inline-block;
                margin-right: 20px;
                padding: 5px;
                border-radius: 5px;

                &.select {
                    border-bottom: 3px solid #038484;
                }

                &:hover {
                    border-bottom: 3px solid #038484;
                    background-color: rgba($color: #d5e7e8, $alpha: 0.5);
                }

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
