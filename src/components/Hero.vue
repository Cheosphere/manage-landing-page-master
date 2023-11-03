<script></script>

<template>
    <section class="container">
        <article class="hero-info">
            <h1 class="hero-title">Bring everyone together to build better products.</h1>
            <p class="hero-text">
                Manage makes it simple for software teams to plan day-to-day
                tasks while keeping the larger team goals in view.
            </p>
            <button>Get Started</button>
        </article>
        <article class="hero-image">
            <figure>
                <img src="../assets/images/illustration-intro.svg" alt="ilustration intro">
            </figure>
        </article>
    </section>
</template>

<style scoped>
.container {
    width: 100%;
    max-width: 1110px;
    display: flex;
    justify-content: space-between;
}
.hero-info {
    width: 50%;
    margin-top: 10.5rem;
}
.hero-title {
    font-size: 3.25rem;
    font-weight: 600;
    line-height: 3.94rem;
    letter-spacing: -.01rem;
    color: var(--dark-blue);
    transition: .3s;
}
.hero-text {
    width: 345px;
    margin-top: 1.9rem;
    font-weight: 200;
    line-height: 1.6rem;
    letter-spacing: .005rem;
    color: var(--dark-grayish-blue);
}
.hero-image {
    width: 50%;
    margin-top: 6.3rem;
    margin-right: .3rem;
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

@media screen and (max-width: 980px) {
    .hero-title {
        font-size: 3rem;
        line-height: 3.8rem;
    }
}

@media screen and (max-width: 960px) {
    .container {
        flex-direction: column-reverse;
        align-items: center;
    }
    .hero-image {
        width: 100%;
        margin-top: 3rem;
        margin-right: 0;
        display: flex;
        justify-content: center;
    }
    .hero-image img {
        width: 100%;
    }
    .hero-info {
        width: 100%;
        margin-top: 3.5rem;
        text-align: center;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .hero-title {
        font-size: 2.9rem;
        line-height: 3.9rem;
    }
    .hero-text {
        width: 100%;
        max-width: 500px;
        margin-top: 1.9rem;
        line-height: 1.6rem;
    }
}

@media screen and (max-width: 480px) {
    .hero-title {
        font-size: 2.5rem;
        line-height: 3.5rem;
    }
}

@media screen and (max-width: 374px) {
    .hero-title {
        font-size: 2rem;
        line-height: 3rem;
    }
}

</style>