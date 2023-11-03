<script></script>

<template>
    <section class="container">
        <button>Get Started</button>
        <article class="get-started">
            <div class="get-started-wrapper">
                <h2 class="get-started-title">Simplify how your team works today.</h2>
                <button class="btn-white">Get Started</button>
            </div>
        </article>
    </section>
</template>

<style scoped>
.container {
    width: 100vw;
    margin-top: 20.9rem;
    display: flex;
    flex-direction: column;
    align-items: center;
}

button {
    width: 137px;
    height: 44px;
    margin-top: 2.45rem;
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

button:hover {
    opacity: .6;
}
.get-started {
    width: 100%;
    height: 220px;
    margin-top: 11.25rem;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: var(--bright-red);
    background-image: url('../assets/images/bg-simplify-section-desktop.svg');
    background-repeat: no-repeat;
    background-position: 17.7vw 100%;
}
.get-started-wrapper {
    width: 100%;
    max-width: 1112px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    transition: .3s;
}
.get-started-title {
    width: 450px;
    font-size: 2.38rem;
    font-weight: 500;
    line-height: 2.78rem;
    letter-spacing: -.01rem;
    color: var(--very-light-gray);
}
.btn-white {
    width: 137px;
    height: 44px;
    margin-top: 0;
    position: relative;
    left: .2rem;
    font-size: .8rem;
    font-weight: 500;
    letter-spacing: .008rem;
    color: var(--bright-red);
    background-color: var(--very-light-gray);
    border-radius: 44px;
    border: none;
    cursor: pointer;
    box-shadow: 0 12px 12px -5px hsla(0, 0%, 0%, 0.1);
    transition: .3s;
}
.btn-white:hover {
    opacity: 1;
    color: hsla(12, 88%, 59%, 0.5);
}

@media screen and (max-width: 1240px) {
    .get-started {
        background-position: -5.7vw 100%;
    }
    .get-started-wrapper {
        padding: 0 2.5rem;
    }
    .btn-white {
        left: 0;
    }
}

@media screen and (max-width: 1080px) {
    .get-started {
        background-position: -5.7vw 100%;
    }
}

@media screen and (max-width: 960px) {
    .get-started {
        height: 405px;
        margin-top: 5rem;
        background-image: url('../assets/images/bg-simplify-section-mobile.svg');
        background-position: 0 3rem;
    }
    .get-started-wrapper {
        height: 50%;
        flex-direction: column;
        text-align: center;
    }    
    .get-started-title {
        width: 100%;
        max-width: 450px;
        font-size: 2.38rem;
        font-weight: 500;
        line-height: 2.78rem;
        letter-spacing: -.01rem;
        color: var(--very-light-gray);
    }

    button {
        margin-top: 5rem;
    }
}

@media screen and (max-width: 420px) {
    .get-started-wrapper {
        height: 50%;
        padding: 0 1.5rem;
        flex-direction: column;
        text-align: center;
    }   
}

@media screen and (max-width: 374px) {
    .get-started-title {
        font-size: 2rem;
    }   
}

</style>