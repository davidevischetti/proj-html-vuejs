<template>
<section class="container">
    <div>
        <h5>WE DO MORE FOR EVERYONE</h5>
        <h2>Actions &amp;<div class="special-text">Projects</div></h2>
    </div>

    <div id="projects-list-links">
        <a v-for="(link,index) in projectsLinks" @click="activeLinkFunc(link)" :key="index" :class="link.active ? 'select' : ''">
        {{link.text}}
        </a>           
    </div>

    <div id="projects-list">
        <ProjectsCard v-for="(project,i) in projectsList" :key="i" :addProject="project"/>
    </div>


</section>
</template>

<script>
import ProjectsCard from './ProjectsCard.vue';
export default {
    name: "ProjectsSection",
    components: { ProjectsCard },
    data () {
        return {
            projectsLinks : [
                {
                    text :'ALL',
                    active : true
                },
                {
                    text : 'INSTITUTIONAL',
                    active : false
                },
                {
                    text : 'SOCIAL',
                    active : false
                },
                {
                    text : 'EVENTS',
                    active : false
                },
                {
                    text : 'INNOVATION',
                    active : false
                },
                {
                    text : 'ENVIRONMENT',
                    active : false
                },
                {
                    text : 'TECHNOLOGY',
                    active : false
                },

            ],
            projectsList : [
                {
                    img: require('../assets/img/project-1.jpg'),
                    text: 'Academic professional program in social media',
                    info: 'Academic professional program in social media'
                },
                {
                    img: require('../assets/img/project-2.jpg'),
                    text: "President's speech at the annual meeting",
                    info: 'Academic professional program in social media'
                },
                {
                    img: require('../assets/img/project-3.jpg'),
                    text: 'International business trip in Shanghai',
                    info: 'Academic professional program in social media'
                },
                {
                    img: require('../assets/img/project-4.jpg'),
                    text: 'Technology workshop with education theme',
                    info: 'Academic professional program in social media'
                },
                {
                    img: require('../assets/img/project-5.jpg'),
                    text: 'Donation of clothes and food to the partner NGO',
                    info: 'Academic professional program in social media'
                },
                {
                    img: require('../assets/img/project-6.jpg'),
                    text: 'Confraternization of the procurement team',
                    info: 'Academic professional program in social media'
                },
            ]
        }
    },

    methods : {
        activeLinkFunc (activeLink) {
            this.projectsLinks.forEach(element => {
            element.active = false
            });

            activeLink.active = true
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
    flex-direction: column;

    h5 {
        color: #54b0c1;
        text-align: center;
        margin-top: 100px;
    }

    h2 {
        font-size: 40px;
        width: 100%;
        text-align: center;
        margin: 20px 0;

        .special-text {
            color: #058283;
            background-color: #d5e7e8;
            margin-left: 10px;
        }

    }

    #projects-list-links {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        width: 100%;
        margin: 30px 0;

        a {
            color: #777;
            font-size: 15px;
            font-weight: 600;
            padding: 5px;
            border-radius: 5px;
            cursor: pointer;

            &.select {
                border-bottom: 3px solid #038484;
            }

            &:hover {
                background-color: #d5e7e8;
                border-bottom: 3px solid #038484;
            }
        }

    }

    #projects-list {
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        width: 100%;
    }
}

</style>
