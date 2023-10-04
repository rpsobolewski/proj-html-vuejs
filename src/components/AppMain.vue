<script>
import AppMainGrid from './AppMainGrid.vue';
import AppMainWork from './AppMainWork.vue';


export default {
    name: 'AppMain',
    components: {
        AppMainGrid,
        AppMainWork


    },
}
</script>
<template>
    <AppMainGrid></AppMainGrid>
    <AppMainWork></AppMainWork>
</template> 
<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
</style>