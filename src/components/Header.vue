<script setup>
import { ref } from 'vue'

const isActive = ref(false)
const isClose = ref(false)
const isShadow = ref(false)

const showMenu = () => {
    isClose.value = !isClose.value
    isActive.value = !isActive.value
    isShadow.value = !isShadow.value
}

</script>

<template>
    <header class="header">
        <figure>
            <img src="../assets/images/logo.svg" alt="logo image">
        </figure>
        <nav class="nav-menu">
            <ul :class="{ active: isActive }" class="menu">
                <li class="item-menu"><a href="javascript:;">Pricing</a></li>
                <li class="item-menu"><a href="javascript:;">Product</a></li>
                <li class="item-menu"><a href="javascript:;">About Us</a></li>
                <li class="item-menu"><a href="javascript:;">Careers</a></li>
                <li class="item-menu"><a href="javascript:;">Community</a></li>
            </ul>
            <span @click="showMenu" :class="{ close: isClose }" class="icon-menu"></span>
        </nav>
        <button>Get Started</button>
    </header>
    <div :class="{ shadow: isShadow }"></div>
</template>

<style scoped>
.header {
    width: 100%;
    max-width: 1110px;
    padding-top: 4.1rem;
    display: flex;
    justify-content: space-between;
    z-index: 10;
}
.menu {
    display: flex;
    position: relative;
    bottom: .5rem;
    right: .35rem;
}
.item-menu {
    display: flex;
    align-items: center;
    list-style: none;
}
.icon-menu {
    width: 26px;
    height: 18px;
    display: none;
    background-image: url('../assets/images/icon-hamburger.svg');
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center;
    cursor: pointer;
    transition: .3s;
}

a {
    margin: 0 1rem;
    font-size: .78rem;
    letter-spacing: .005rem;
    text-decoration: none;
    color: var(--dark-blue);
    transition: .3s;
}

button {
    width: 137px;
    height: 44px;
    position: relative;
    bottom: .6rem;
    font-size: .8rem;
    font-weight: 500;
    letter-spacing: .008rem;
    color: var(--very-pale-red);
    background-color: var(--bright-red);
    border-radius: 44px;
    border: none;
    cursor: pointer;
    box-shadow: 0 12px 12px -5px hsla(12, 88%, 59%, 0.5);
    transition: .3s;
}

a:hover,
button:hover {
    opacity: .6;
}

@media screen and (max-width: 960px) {
    .header {
        position: relative;
    }
    .menu {
        width: 100%;
        height: 290px;
        flex-direction: column;
        align-items: center;
        justify-content: space-evenly;
        position: absolute;
        top: -22rem;
        left: 0;
        background-color: white;
        border-radius: 8px;
        transition: .3s ease-out;
    }
    .icon-menu {
        display: block;
    }

    a {
        font-size: 1rem;
        font-weight: 600;
    }

    button {
        display: none;
    }
    .active {
        top: 8rem;
    }
    .close {
        background-image: url('../assets/images/icon-close.svg');
        transform: rotate(180deg);
        transition: .5s;
    }
    .shadow {
        position: absolute;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        background: linear-gradient(0deg, rgba(0, 0, 0, 1) 0%, rgba(0, 0, 0, 0) 100%);
        z-index: 8;
    }
}

@media screen and (max-width: 480px) {
    .header {
        padding-top: 3rem;
    }
}

</style>