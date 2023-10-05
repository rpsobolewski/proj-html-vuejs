<template>
    <div class="d-flex justify-content-center">
        <div class="col-3"><!-- card 1 -->
            <div class="banner"><!-- banner -->

                <p class="date">07</p>
                <span class="year">MAY '19</span>
            </div>

            <img src="../assets/h-2-blog-img-1.jpg" alt="">
            <h2>This way, loves: a detailed guide through new design</h2>
            <p>By Emily Fields</p>
        </div>
        <div class="col-3"><!-- card 2 -->
            <div class="banner"><!-- banner -->

                <p class="date">07</p>
                <span class="year">MAY '19</span>
            </div>

            <img src="../assets/h-2-blog-img-2.jpg" alt="">
            <h2>I try to give people a different way of looking at art</h2>
            <p>By Emily Fields</p>
        </div>
        <div class="col-3"><!-- card 3 -->
            <div class="banner"><!-- banner -->

                <p class="date">07</p>
                <span class="year">MAY '19</span>
            </div>

            <img src="../assets/h-2-blog-img-3.jpg" alt="">
            <h2>introduce Richard Laperrière of those amazing features</h2>
            <p>By Emily Fields</p>
        </div>


    </div>
</template>

<script >
export default {
    name: 'AppMainEvents'
}
</script>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

img {
    width: 100%;
    position: relative;
    z-index: 1;

}

p {
    font-family: 'Lobster', cursive;
}

.date {
    font-size: 40px;
    margin-bottom: -10px;
    background-color: $m_backgroundDarkGreen;
    width: 70px;
    text-align: center;

}

.year {
    background-color: $m_backgroundPink;
    padding: 0 6px;
    padding-bottom: 20px;
    clip-path: polygon(0 0, 100% 0, 100% 100%, 50% 80%, 0 100%);

}

.banner {
    margin-left: 10px;
    margin-bottom: -50px;
    padding-top: 30px;
    position: relative;
    z-index: 2;

}


.col-3 {
    margin: 0 8px;
}
</style>