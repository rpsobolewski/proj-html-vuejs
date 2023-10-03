<script>


export default {
    name: 'AppHeaderNavbar',
    data() {
        return {
            navItems: ['HOME', 'PAGES', 'PORTFOLIO', 'BLOG', 'GAMES', 'SHOP', 'ELEMENTS'],
            activeIndex: null,
        };
    },

}
</script>
<template>
    <div class="d-flex justify-content-between p-3">
        <img class="logo" src="../assets/logo-sidearea-1.png" alt="">
        <div>
            <ul class="nav justify-content-center ">
                <li class="nav-item" v-for="(item, index) in navItems" :key="index">
                    <a class="nav-link" aria-current="page" href="#">{{ item }}</a>
                </li>

                <svg class="" xmlns="http://www.w3.org/2000/svg" width="23" height="23">
                    <circle cx="3" cy="20.1" r="2" />
                    <circle cx="11.7" cy="20.1" r="2" />
                    <circle cx="20.2" cy="20.1" r="2" />
                    <circle cx="3" cy="2.9" r="2" />
                    <circle cx="11.7" cy="2.9" r="2" />
                    <circle cx="20.2" cy="2.9" r="2" />
                    <circle cx="3" cy="11.4" r="2" />
                    <circle cx="11.7" cy="11.4" r="2" />
                    <circle cx="20.2" cy="11.4" r="2" />
                </svg>



            </ul>
        </div>
    </div>
</template> 
<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

* {
    font-family: 'Anton', sans-serif;
    font-family: 'Fira Sans', sans-serif;
    font-family: 'Montserrat', sans-serif;
}

.nav-link {
    color: $m_dark;
    margin-bottom: -50px;
    font-weight: 400;
    font-size: 14px;
    padding: 25px;

}




li:hover {
    border-bottom: 6px solid $m_navUnderline;
    margin-bottom: 4px;
}

svg {
    margin-top: 25px;
}

svg:hover {
    fill: $m_navUnderline;
}

.logo {
    padding-left: 10px;
    object-fit: contain;
}
</style>