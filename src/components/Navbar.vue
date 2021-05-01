<template>
            <nav class="nav-menu">
            <a href="#" class="logo">logo</a>
            <ul class="nav-list">
                <li class="nav-item">
                    <a href="#intro" class="nav-link">skillz.</a>
                </li>
                <li class="nav-item">
                    <a href="" class="nav-link">projects.</a>
                </li>
                <li class="nav-item">
                    <a href="" class="nav-link">about-me.</a>
                </li>
                <li class="nav-item">
                    <a href="" class="nav-link">contact.</a>
                </li>
            </ul>
        </nav>
</template>

<script>

export default {
  name: 'Navbar'
}
</script>

<style lang="scss">
@import '../scss/config';
.nav-menu {
    display: flex;
    justify-content: space-between;
    padding: 40px 0px;

    .nav-list {
        margin: 0;
        padding: 0;
        list-style: none;
        .nav-item{
            display: inline-block;
            padding-right: 25px;
            &:last-of-type {
                padding-right: 0;  
            }
            .nav-link {
                text-decoration: none;
                font-size: 1.125rem;
                font-weight: 500;
                font-family: $raleway;
                color:$darkBlue;
                transition: all .3s ease;
                &:hover {
                    color:$lightBlue;
                }
            }
        }
    }
}
</style>
