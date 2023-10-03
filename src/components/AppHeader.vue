<script>
import AppHeaderNavbar from './AppHeaderNavbar.vue';


export default {
    name: 'AppHeader',
    components: {
        AppHeaderNavbar
    },
    data() {
        return {
            navItems: ['HOME', 'PAGES', 'PORTFOLIO', 'BLOG', 'GAMES', 'SHOP', 'ELEMENTS']
        }
    },
}
</script>
<template>
    <AppHeaderNavbar v-bind:navItems="navItems"></AppHeaderNavbar>
    AppHeader
</template> 
<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
</style>