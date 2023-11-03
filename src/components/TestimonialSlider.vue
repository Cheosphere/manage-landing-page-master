<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Autoplay, Pagination } from 'swiper/modules';
// Import Swiper styles
import 'swiper/css';
import 'swiper/css/pagination';

const modules = [Autoplay, Pagination];

const testimonialData = [
    {
        name: 'Anisha Li',
        text: '"Manage has supercharged our team’s workflow. The ability to maintain visibility on larger milestones at all times keeps everyone motivated."',
        src: '/manage-landing-page-master/assets/avatar-anisha.png'
    },
    {
        name: 'Ali Bravo',
        text: '“We have been able to cancel so many other subscriptions since using Manage. There is no more cross-channel confusion and everyone is much more focused.”',
        src: '/manage-landing-page-master/assets/avatar-ali.png'
    },
    {
        name: 'Richard Watts',
        text: '“Manage allows us to provide structure and process. It keeps us organized and focused. I can’t stop recommending them to everyone I talk to!”',
        src: '/manage-landing-page-master/assets/avatar-richard.png'
    },
    {
        name: 'Shanai Gough',
        text: '“Their software allows us to track, manage and collaborate on our projects from anywhere. It keeps the whole team in-sync without being intrusive.”',
        src: '/manage-landing-page-master/assets/avatar-shanai.png'
    }
]
</script>

<template>
    <h2 class="testimonial-title">What they’ve said</h2>
    <section>
        <swiper
            :slidesPerView="3"
            :grabCursor="true"
            :loop="true"
            :spaceBetween="30"
            :centeredSlides="false"
            :pagination="true"
            :autoplay="{
                delay: 3500,
                disableOnInteraction: false,
                pauseOnMouseEnter: true
            }"
            :modules="modules"
            class="mySwiper">
            <swiper-slide v-for="item in testimonialData" :key="item.name">
                <article class="card">
                    <figure>
                        <img :src="item.src" :alt="item.name">
                    </figure>
                    <h5>{{ item.name }}</h5>
                    <p>{{ item.text }}</p>
                </article>
            </swiper-slide>
        </swiper>
    </section>
</template>

<style scoped>
section {
    width: 100vw;
    display: flex;
    justify-content: center;
    position: relative;
}
.testimonial-title {
    margin-top: 9.2rem;
    font-size: 2.4rem;
    font-weight: 600;
    letter-spacing: -.02rem;
    color: var(--dark-blue);
}
.swiper {
    width: 1675px;
    height: fit-content;
    position: absolute;
}
.swiper-slide {
    width: 100%;
    height: 220px;
    margin-top: 6.55rem;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    text-align: center;
    background-color: var(--very-light-gray);
}
.swiper-slide img {
    display: block;
    width: 72px;
    height: 72px;
    object-fit: cover;
    position: absolute;
    top: 0;
    left: 50%;
    transform: translate(-50%, -50%);
}
.card {
    padding: 2.5rem;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.card h5 {
    margin-top: .3rem;
    font-size: .95rem;
    font-weight: 600;
    color: var(--dark-blue);
}
.card p {
    position: relative;
    top: 1.2rem;
    font-size: .97rem;
    font-weight: 200;
    line-height: 1.65rem;
    letter-spacing: .02rem;
    color: var(--dark-grayish-blue);
}

@media screen and (max-width: 960px) {
    .testimonial-title {
        margin-top: 5rem;
    }
}

@media screen and (max-width: 580px) {
    .swiper {
        width: 300%;
    }
    .card {
        padding: 1rem;
    }
}

@media screen and (max-width: 480px) {
    .testimonial-title {
        font-size: 2rem;
        text-align: center;
    }
}

</style>