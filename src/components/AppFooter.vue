<script>


export default {
    props: ['footerItems'],
    name: 'AppFooter'
}
</script>

<template>
    <div class="d-flex justify-content-center p-5">
        <div class="col margin">

            <img class="ps-2 pb-2" :src="footerItems.img" alt="">
            <div>{{ footerItems.motto }}</div>

        </div>
        <div class="col margin">

            <div class=" pb-2">{{ footerItems.email }}</div>

            <div>{{ footerItems.number }}</div>

        </div>
        <div class="col margin">

            <div class=" pb-2">{{ footerItems.address1 }}</div>

            <div>{{ footerItems.address2 }}</div>

        </div>
        <div class="col margin">

            <div class=" pb-2">{{ footerItems.message }}</div>


            <div class="d-flex ">

                <div class="p-2 ps-4" v-html="footerItems.social1"></div>
                <div class="p-2" v-html="footerItems.social2"></div>
                <div class="p-2" v-html="footerItems.social3"></div>
                <div class="p-2" v-html="footerItems.social4"></div>
            </div>


        </div>


    </div>
</template> 
<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

* {
    background-color: $m_backgroundDarkGreen;
}

.margin {
    margin: 0 20px;
}

.col {
    max-width: 250px;
}
</style>