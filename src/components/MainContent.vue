<script></script>

<template>
    <main class="container">
        <div class="pattern"></div>
        <article class="content-left">
            <h2 class="content-left-title">What’s different about Manage?</h2>
            <p class="content-left-text">
                Manage provides all the functionality your team needs, without
                the complexity. Our software is tailor-made for modern digital
                product teams.
            </p>
        </article>
        <article class="content-right">
            <div class="content-right-item">
                <div class="content-right-item-info">
                    <span>01</span>
                    <h4>Track company-wide progress</h4>
                </div>
                <p>
                    See how your day-to-day tasks fit into the wider vision. Go from
                    tracking progress at the milestone level all the way done to the
                    smallest of details. Never lose sight of the bigger picture again.
                </p>
            </div>
            <div class="content-right-item">
                <div class="content-right-item-info">
                    <span>02</span>
                    <h4>Advanced built-in reports</h4>
                </div>
                <p>
                    Set internal delivery estimates and track progress toward company
                    goals. Our customisable dashboard helps you build out the reports
                    you need to keep key stakeholders informed.
                </p>
            </div>
            <div class="content-right-item">
                <div class="content-right-item-info">
                    <span>03</span>
                    <h4>Everything you need in one place</h4>
                </div>
                <p>
                    Stop jumping from one service to another to communicate, store files,
                    track tasks and share documents. Manage offers an all-in-one team
                    productivity solution.
                </p>
            </div>
        </article>
    </main>
</template>

<style scoped>
.container {
    width: 100%;
    max-width: 1110px;
    margin-top: 6.4rem;
    display: flex;
    position: relative;
}
.pattern {
    width: 100%;
    height: 200%;
    position: absolute;
    top: 9.7rem;
    right: 60.25%;
    background-image: url('../assets/images/bg-tablet-pattern.svg');
    background-repeat: no-repeat;
    background-position: left;
    z-index: -10;
}

.content-left,
.content-right {
    width: 50%;
    transition: .3s;
}
.content-left-title {
    font-size: 2.4rem;
    font-weight: 600;
    line-height: 2.7rem;
    letter-spacing: -.025rem;
    color: var(--dark-blue);
}
.content-left-text {
    max-width: 340px;
    margin-top: 1.85rem;
    font-weight: 200;
    line-height: 1.62rem;
    letter-spacing: .005rem;
    color: var(--dark-grayish-blue);
}
.content-right {
    margin-top: -.35rem;
    padding-left: .95rem;
}
.content-right-item:nth-child(2) {
    margin-top: 2.45rem;
}
.content-right-item:nth-child(3) {
    margin-top: 2.43rem;
}
.content-right-item span {
    min-width: 67px;
    height: 39px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: 500;
    border-radius: 39px;
    color: var(--very-light-gray);
    background-color: var(--bright-red);
}
.content-right-item-info {
    width: 100%;
    display: flex;
    align-items: center;
}
.content-right-item-info h4 {
    margin-left: 1.7rem;
    font-size: .97rem;
    font-weight: 600;
    letter-spacing: -.027rem;
    color: var(--very-dark-blue);
}
.content-right-item p {
    max-width: 440px;
    margin-left: 5.9rem;
    margin-top: .65rem;
    font-size: .96rem;
    font-weight: 200;
    line-height: 1.62rem;
    letter-spacing: .02rem;
    color: var(--dark-grayish-blue);
}
.content-right-item:nth-child(2) h4 {
    letter-spacing: -.02rem;
}
.content-right-item:nth-child(3) h4 {
    letter-spacing: -.017rem;
}
.content-right-item:nth-child(2) p {
    letter-spacing: .025rem;
}
.content-right-item:nth-child(3) p {
    letter-spacing: .027rem;
}

@media screen and (max-width: 1080px) {
    .content-left {
        width: 47%;
    }
    .content-left-text {
        max-width: 400px;
        margin-top: 1.85rem;
        font-weight: 200;
        line-height: 1.62rem;
        letter-spacing: .005rem;
        color: var(--dark-grayish-blue);
    }
    .content-right {
        width: 53%;
        margin-top: 0;
        padding-left: 0;
    }
}

@media screen and (max-width: 980px) {
    .content-left-title {
        font-size: 2.2rem;
    }
}

@media screen and (max-width: 960px) {
    .container {
        max-width: none;
        margin-top: 6.4rem;
        flex-direction: column;
        align-items: center;
    }
    .content-left,
    .content-right {
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .content-left {
        text-align: center;
    }
    .content-left-text {
        width: 100%;
        max-width: 600px;
    }
    .content-right {
        margin-top: 5rem;
    }
    .content-right-item-info {
        border-radius: 39px 0 0 39px;
        background-color: hsl(12, 88%, 59%, .12);
    }
    .content-right-item p {
        width: 100%;
        max-width: 440px;
        margin-left: 0;
        margin-top: .65rem;
        font-size: .96rem;
        font-weight: 200;
        line-height: 1.62rem;
        letter-spacing: .02rem;
        color: var(--dark-grayish-blue);
    }
    .pattern {
        top: -130%;
        right: -30%;
        background-position: right;
        background-size: 50%;
    }
}

@media screen and (max-width: 480px) {
    .content-right-item-info {
        width: 110%;
    }
    .content-left-title {
        font-size: 2rem;
    }
}

@media screen and (max-width: 540px) {
    .pattern {
        top: -120%;
        right: -55%;
        background-size: 90%;
    }
}

@media screen and (max-width: 374px) {
    .content-right-item span {
        min-width: 50px;
    }
    .content-right-item-info h4 {
        margin-left: .5rem;
        font-size: .9rem;
    }
}

</style>