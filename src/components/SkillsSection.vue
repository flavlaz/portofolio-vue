<template>
    <section id="skills" class="pb-30">
            <div class="item" v-for="skill in skills" v-bind:key="skill.id">
                    <h1 class="title mb-35"> {{ skill.title }} </h1>
                    <span class="desc mb-60"> {{ skill.desc }} </span>
                    <h2 class="subtitle"> {{ skill.subtitle }} </h2>
                    <span class="desc mb-60"> {{ skill.subdesc }}</span>
                    <h2 class="subtitle"> {{ skill.toolstitle }} </h2>
                    <span class="desc"> {{ skill.tools }}</span>
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
        padding: 45px 25px;
        border:1px solid #DEDEDE;
        background-color:#ffffff;
        .title {
            font-family: $raleway;
            font-size: 1.75rem;
            font-weight: bold;
            color:$darkBlue;
        }
        .subtitle{
            font-family: $raleway;
            font-size: 1.375rem;
            color: $lightBlue;
            font-weight: 500;
        }
        .desc {
            font-family: $poppins;
            font-size: 1.125rem;
        }
        span {
            display: block;
        }
        &:first-of-type{
            border-top-left-radius:15px;
            border-bottom-left-radius:15px;
        }
        &:last-of-type{
            border-top-right-radius:15px;
            border-bottom-right-radius:15px;
        }
    }
}
@media screen and(max-width:415px) {
    #skills {
        flex-direction: column;
    }
}
</style>
