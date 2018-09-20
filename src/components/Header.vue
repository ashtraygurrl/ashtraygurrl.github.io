<template>
<header class="hero is-fullheight">
    <div class="hero-head">
        <nav class="navbar">
            <div class="container">
                <div class="navbar-end">
                    <a class="navbar-item active" href="#">home</a>
                    <a class="navbar-item" href="#">gallery</a>
                    <a class="navbar-item" href="#">contact</a>              
                </div>
            </div>    
        </nav>
    </div>
    <section class="hero-body">
        <nav class="social-icons">
            <a href="#">
                <span class="icon-facebook"></span>
            </a>
            <a href="#">
                <span class="icon-instagram"></span>
            </a>
            <a href="#">
                <span class="icon-spotify"></span>
            </a>
        </nav>
        <div class="container">
            <h1 class="title name"> Guadalupe</h1>
        </div>
    </section>
</header>
</template>
<style lang="scss" scoped>
@import '../styles/_colors';
@import '../styles/_icons';
@import '~bulma/bulma.sass';

.hero {
    background-color: $white;

    &-body {
        position: relative;
    }

    &-body {
        height: 100%;
    }
}

.name {
    font-family: 'RNS Miles', sans-serif;
    font-size: 120px;
    text-transform: uppercase;
    letter-spacing: 24px;
}

a.navbar-item {
    background-color: transparent;
    color: $black;
    font-family: 'RNS Miles', sans-serif;
    font-size: 50px;
    position: relative;
    text-decoration: none;
    transition: transform 150ms ease-in;

    &:hover {
        background-color: transparent;
        color: $black;
        transform: scale(1.05);
    }

    &.active:before {
        background-color: $black;
        box-sizing: border-box;
        content: '';
        display: block;
        height: 3px;
        left: 50%;
        position: absolute;
        top: 40%;
        width: 100%;
        transform: rotate(-10deg) translate(-50%, -50%);
        transform-origin: 50% 50%;
    }
}

.social-icons {
    display: flex;
    flex-direction: column;
    left: 0;
    position: absolute;
    top: 40px;
    font-size: 80px;

    a {
        color: $black;
    }
}
</style>
