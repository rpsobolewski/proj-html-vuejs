<template>
    <div class="d-flex flex-wrap mt-5">
        <div class="col-4"><img src="../assets/h-2-port-img-1.jpg" alt=""></div>
        <div class="col-4"><img src="../assets/h-2-port-img-2.jpg" alt=""></div>
        <div class="col-4"><img src="../assets/h-2-port-img-3.jpg" alt=""></div>
        <div class="col-4"><img src="../assets/h-2-port-img-4.jpg" alt=""></div>
        <div class="col-4"><img src="../assets/h-2-port-img-5.jpg" alt=""></div>
        <div class="col-4"><img src="../assets/h-2-port-img-6.jpg" alt=""></div>
    </div>
</template>

<script >
export default {
    name: 'AppMainGrid'
}
</script>

<style lang="scss" scoped>
.col-4 {

    object-fit: contain;
}

img {
    width: 100%;

}
</style>