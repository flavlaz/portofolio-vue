<template>
    <section id="skills">
            <div class="item" v-for="skill in skills" v-bind:key="skill.id">
                <div class="box upper-box">
                    <h1 class="title"> {{ skill.title }} </h1>
                    <span class="desc"> {{ skill.desc }} </span>
                </div>
                <div class="box middle-box">
                    <h2> {{ skill.subtitle }} </h2>
                    <span> {{ skill.subdesc }}</span>
                </div>
                <div class="box bottom-box">
                    <h2> {{ skill.toolstitle }} </h2>
                    <span> {{ skill.tools }}</span>
                </div>
            </div>
    </section>
</template>

<script>

export default {
  name: 'SkillsSection',
  data () {
      return {
      skills:[
          {
            title: 'Design',
            desc: 'I value simple content structure, clean design patterns, and thoughtful interactions.',
            subtitle:'Things I enjoy designing:',
            subdesc:'UX, UI, Web, Mobile, Apps, Logos',
            toolstitle:'Design Tools:',
            tools:'Illustrator, Photoshop, Adobe XD'
          },
          {
            title: 'Development',
            desc: 'I like to code things from scratch, and enjoy bringing ideas to life in the browser.',
            subtitle:'Languages I speak:',
            subdesc:'HTML, CSS, Scss, Vue JS, Php',
            toolstitle:'Dev Tools:',
            tools:'VS Code, Bootstrap, Github, Vue CLI ' 
          },
          {
            title: 'SEO Optimization',
            desc: 'I value simple content structure, clean design patterns, and thoughtful interactions.',
            subtitle:'Tool used for seo audit:',
            subdesc:'G.Analitics, P.Speed Insight, GT Metrix',
            toolstitle:'Seo Tools:',
            tools:'KeyWord, HeadingOrder, Db.Content' 
          }
        ]
    }
  } 
}
</script>

<style lang="scss">
@import '../scss/config';
#skills {
    display: flex;
    margin-top: -10%;
    .item {
        flex:1;
        text-align: center;
        padding: 30px 15px;
        border:1px solid #DEDEDE;
        background-color:#ffffff;
        .middle-box {
            padding: 30px 15px;
        }
        .title {
            font-family: $raleway;
            font-size: 1.5rem;
            font-weight: bold;
            color:$darkBlue;
        }
    }
}
</style>
