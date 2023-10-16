<template>
    <nav class="navbar" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
            <a class="navbar-item" href="https://bulma.io">
                <img src="../assets/dashboard.png" width="120" height="30">
            </a>

            <a role="button" class="navbar-burger" ref="burger" @click="openHamburger" aria-label="menu"
                aria-expanded="false" data-target="navbarBasicExample">
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
            </a>
        </div>

        <div id="navbarBasicExample" class="navbar-menu" ref="menu">
            <div class="navbar-start">
                <a class="navbar-item">
                    Home
                </a>

                <a class="navbar-item">
                    Price Feed
                </a>

                <a class="navbar-item">
                    Gymbrah Schedule
                </a>

                <a class="navbar-item">
                    Manga Updates
                </a>

                <a class="navbar-item">
                    カタカナ
                </a>
            </div>

        </div>
    </nav>
</template>
  
<script>

import { ref } from 'vue';

export default {
    name: 'NavBar',
    setup() {
        // Create refs for DOM elements
        const burger = ref(null);
        const menu = ref(null);

        const openHamburger = () => {
            menu.value.classList.toggle('is-active');
        };


        return {
            burger,
            menu,
            openHamburger
        };
    },
}
</script>
<style>
.navbar,
.navbar-menu {
    background-color: #FFF2F1;
}
</style>  
  