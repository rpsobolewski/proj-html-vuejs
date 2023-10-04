<script>
import AppMainGrid from './AppMainGrid.vue';
import AppMainWork from './AppMainWork.vue';
import AppMainBanner from './AppMainBanner.vue';



export default {
    name: 'AppMain',
    components: {
        AppMainGrid,
        AppMainWork,
        AppMainBanner



    },
}
</script>
<template>
    <AppMainGrid></AppMainGrid>
    <AppMainWork></AppMainWork>
    <AppMainBanner></AppMainBanner>
</template> 
<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
</style>