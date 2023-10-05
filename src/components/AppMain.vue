<script>
import AppMainGrid from './AppMainGrid.vue';
import AppMainWork from './AppMainWork.vue';
import AppMainBanner from './AppMainBanner.vue';
import AppMainEvents from './AppMainEvents.vue';




export default {
    name: 'AppMain',
    components: {
        AppMainGrid,
        AppMainWork,
        AppMainBanner,
        AppMainEvents



    },
}
</script>
<template>
    <AppMainGrid></AppMainGrid>
    <AppMainWork></AppMainWork>
    <AppMainBanner></AppMainBanner>
    <AppMainEvents></AppMainEvents>
</template> 
<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
</style>