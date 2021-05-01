<template>
    <section id="projects" class="p-30">
        <h2 class="title">Some recent projects i've worked on</h2>
        <p class="subtitle">Here are a few design projects I've worked on recently. Want to see more? Email me.</p>
        <div class="projects-wrapper">
            <div class="project-item" v-for="project in projects" v-bind:key="project.id">
                <img :src="project.img" alt="">
                <p>{{project.desc}}</p>
            </div>
        </div>
    </section>
</template>

<script>


export default {
    name: 'ProjectsSection',
    data(){
        return{
            projects:[
                {   
                    id:1,
                    img:'img/logo.png',
                    desc:'descriere 1'
                },
                {
                    id:2,
                    logo:'',
                    desc:'descriere 2'
                },
                {
                    id:3,
                    logo:'',
                    desc:'descriere 3'
                },
                {
                    id:4,
                    logo:'',
                    desc:'descriere 4'
                },
                {
                    id:5,
                    logo:'',
                    desc:'descriere 5'
                },
                {
                    id:6,
                    logo:'',
                    desc:'descriere 6'
                }
            ]
        }
    }
}
</script>

<style lang="scss">
@import '../scss/config';
#projects {
    text-align: center;
    .project-item {
        width: calc(100%/3);
        display: inline-block;
    }
}

</style>