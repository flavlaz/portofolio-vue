<template>
    <section id="hero" class="container">
        <div class="hero-content-wrapper">
            <h1 class="hero-heading">Front End Developer with<br> an eye for Design</h1>
            <span class="hero-subheading">I create simple yet beautiful websites and webapps</span>
        </div>
        <div class="hero-img-wrapper">
            <img src="../assets/hero-resized.png" alt="">
        </div>
    </section>
</template>

<script>

export default {
  name: 'HeroSection'
}
</script>

<style lang="scss">
@import '../scss/config';
#hero {
    display: flex;
    flex-direction: column;
    height: calc(100vh - 100px);
    justify-content: space-between;
    .hero-img-wrapper {
        display: flex;
        justify-content: center;
        img{
            max-width: 100%;
        }
    }
    .hero-content-wrapper {
        display: flex;
        flex-direction: column;
        flex:1;
        justify-content: center;
        text-align: center;
        padding-bottom: 80px;
        .hero-heading{
            font-size: 3rem;
            font-family: $raleway;
            color:$darkBlue;
            font-weight: 700;
            margin-bottom: 25px;
            line-height: 1.2;
            letter-spacing: -1px;
        }
        .hero-subheading{
            color: $darkBlue;
            font-size: 1.5rem;
            font-family: $poppins;
            font-weight: 300;
        }
    }
}


</style>
