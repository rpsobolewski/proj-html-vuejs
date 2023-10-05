<script>
import AppHeaderNavbar from './AppHeaderNavbar.vue';




export default {

    name: 'AppHeader',
    components: {
        AppHeaderNavbar,


    },
    data() {
        return {
            navItems: ['HOME', 'PAGES', 'PORTFOLIO', 'BLOG', 'GAMES', 'SHOP', 'ELEMENTS'],
            currentSlide: 0,
        }
    },
    methods: {

        prevSlide() {
            this.currentSlide = (this.currentSlide - 1 + 3) % 3;
        },

        nextSlide() {
            this.currentSlide = (this.currentSlide + 1) % 3;
        },
    },
}
</script>
<template>
    <AppHeaderNavbar v-bind:navItems="navItems"></AppHeaderNavbar>

    <div class="slider d-flex justify-content-end">
        <div class="col-1"><!-- prev button -->
            <div class="button" @click="prevSlide">
                <svg xmlns="http://www.w3.org/2000/svg" height="1em"
                    viewBox="0 0 320 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. -->
                    <path
                        d="M9.4 233.4c-12.5 12.5-12.5 32.8 0 45.3l192 192c12.5 12.5 32.8 12.5 45.3 0s12.5-32.8 0-45.3L77.3 256 246.6 86.6c12.5-12.5 12.5-32.8 0-45.3s-32.8-12.5-45.3 0l-192 192z" />
                </svg>

            </div>

        </div>

        <div class="col-4">
            <h1 class="title_1 d-inline">Devotion that never </h1>
            <h1 class="title_2 d-inline ">ends</h1>
            <p class="pt-3 pb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor ducimus obcaecati cupiditate
                ipsam ab voluptas
                pariatur nemo dolore! Nesciunt, praesentium?</p>
            <a class="readMore" href="#">READ MORE</a>
        </div><!-- text -->
        <div class="col-5"><!-- img -->

            <div class=" slide1" v-if="currentSlide === 0"><img class="position-relative"
                    src="../assets/h-2-slider-img-15.png" alt="">
                <img src="../assets/h-2-slider-img-16.png" alt="">

                <img class="position-absolute foglia_1" src="../assets/h-2-slider-img-12.png" alt="">
                <img class="position-absolute foglia_2" src="../assets/h-2-slider-img-13.png" alt="">
                <img class="position-absolute foglia_3" src="../assets/h-2-slider-img-14.png" alt="">
                <img class="position-absolute foglia_4" src="../assets/h-2-slider-img-17.png" alt="">
                <img class="position-absolute foglia_5" src="../assets/short-slider-rev-1-img-2.png" alt="">
                <img class="position-absolute foglia_6" src="../assets/short-slider-rev-1-img-2.png" alt="">

            </div>
            <div class="slide2 ma" v-else-if="currentSlide === 1">
                <img src="../assets/h-2-slider-img-11.png" alt="">
            </div>
            <div class="slide3 ma" v-else>
                <img src="../assets/short-slider-rev-1-img-3.png" alt="">
            </div>










        </div>
        <div class="col-1 "><!-- next button -->

            <div class="button" @click="nextSlide">

                <svg xmlns="http://www.w3.org/2000/svg" height="1em"
                    viewBox="0 0 320 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. -->
                    <path
                        d="M310.6 233.4c12.5 12.5 12.5 32.8 0 45.3l-192 192c-12.5 12.5-32.8 12.5-45.3 0s-12.5-32.8 0-45.3L242.7 256 73.4 86.6c-12.5-12.5-12.5-32.8 0-45.3s32.8-12.5 45.3 0l192 192z" />
                </svg>

            </div>

        </div>


    </div>
</template> 
<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

img {
    max-height: 430px;
}

.ma {
    margin-left: 100px;
}

.slider {
    padding-top: 70px;
}

svg {
    fill: white;
    padding-bottom: 3px;

}

.button {
    background-color: $m_navUnderline;
    width: 24px;
    text-align: center;
    border-radius: 50%;
    margin-top: 100%;


}

.foglia_1 {
    top: 30%;
    left: 47%;
}

.foglia_2 {
    top: 53%;
    left: 50%;

}

.foglia_6 {
    top: 20%;
    left: 85%;
    rotate: 90deg;

}

.foglia_4 {
    top: 48%;


}

.foglia_5 {

    left: 50%;

}

.foglia_3 {
    top: 10%;
    left: 80%;
}

.title_2,
.title_1 {
    font-size: 85px;

}

.title_2 {
    font-family: 'Lobster', cursive;
}

P {
    color: $m_textDarkGray ;
}

.readMore {
    text-decoration: none;
    color: $m_dark;
    font-family: 'Anton', sans-serif;
    font-family: 'Fira Sans', sans-serif;
    font-family: 'Montserrat', sans-serif;
    border: 2px solid $m_navUnderline;
    padding: 7px 10px;

}
</style>