<template>
    <section id="intro">
        <div class="container">
            <h2 class="title">Hi, I’m Flaviu. Nice to meet you.</h2>
            <p class="subtitle">Since beginning my journey as a freelance designer nearly 10 years ago, I've done remote work for agencies, consulted for startups, and collaborated with talented people to create digital products for both business and consumer use. I'm quietly confident, naturally curious, and perpetually working on improving my chops one design problem at a time.</p>
        </div>
    </section>
</template>

<script>

export default {
  name: 'IntroSection'
}
</script>

<style lang="scss">
@import '../scss/config';

#intro {
    background-color: $lightBlue;
    color:#ffffff;
    text-align: center;
    padding: 100px 0px 200px;
    .subtitle{
        max-width: 800px;
        margin: 0 auto;
    }
}

</style>
