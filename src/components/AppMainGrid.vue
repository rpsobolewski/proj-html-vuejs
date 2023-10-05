<template>
    <div class="d-flex flex-wrap mt-5">
        <div class="col-4"><img src="../assets/h-2-port-img-1.jpg" alt="">
            <div class="hover ps-2">
                <h2>Illustration of novels</h2>
                <p>Illustration</p>
            </div>
        </div>
        <div class="col-4"><img src="../assets/h-2-port-img-2.jpg" alt="">
            <div class="hover ps-2">
                <h2>Illustration of novels</h2>
                <p>Illustration</p>
            </div>
        </div>
        <div class="col-4"><img src="../assets/h-2-port-img-3.jpg" alt="">
            <div class="hover ps-2">
                <h2>Illustration of novels</h2>
                <p>Illustration</p>
            </div>
        </div>
        <div class="col-4"><img src="../assets/h-2-port-img-4.jpg" alt="">
            <div class="hover ps-2">
                <h2>Illustration of novels</h2>
                <p>Illustration</p>
            </div>
        </div>

        <div class="col-4"><img src="../assets/h-2-port-img-5.jpg" alt="">
            <div class="hover ps-2">
                <h2>Illustration of novels</h2>
                <p>Illustration</p>
            </div>
        </div>
        <div class="col-4"><img src="../assets/h-2-port-img-6.jpg" alt="">
            <div class="hover ps-2">
                <h2>Illustration of novels</h2>
                <p>Illustration</p>
            </div>
        </div>
    </div>
</template>

<script >
export default {
    name: 'AppMainGrid'
}
</script>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.col-4 {

    object-fit: contain;
    position: relative;
}

img {
    width: 100%;

}

.hover {
    background-color: rgb(249, 247, 243);
    width: 350px;
    height: 100px;
    position: absolute;
    top: 200px;
    left: 0;
    opacity: 0;

    transition: opacity 0.3s ease-in-out;

}

.col-4:hover .hover {
    opacity: 1;

}

p {
    font-family: 'Lobster', cursive;
    font-size: 20px;

}
</style>