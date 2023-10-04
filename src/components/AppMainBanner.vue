<template>
    <div class="text-center mt-5 wrapper">
        <div class="container">

            <h1 class="title_1 d-inline">Want to work with us? Send us </h1>
            <h1 class="title_2 d-inline ">a message!</h1>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptate mollitia architecto delectus recusandae
                repellendus dolorum quo at nihil atque natus, beatae animi iusto cumque inventore adipisci culpa, ut
                consequuntur dignissimos facere maiores libero vitae quia aliquid. Culpa nemo corrupti magnam.</p>
            <a href="#">CONTACT</a>
        </div>

    </div>
</template>

<script>

export default {
    name: 'AppMainBanner'
}

</script>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;


.wrapper {
    background-image: url(../assets/h-2-background-1.jpg);
    padding: 150px;
}

.title_2,
.title_1 {
    font-size: 65px;


}

.title_2 {
    font-family: 'Lobster', cursive;
}



p {
    color: $m_textMidGray;
    margin: 40px;
}

a {
    font-family: 'Anton', sans-serif;
    font-family: 'Fira Sans', sans-serif;
    font-family: 'Montserrat', sans-serif;
    text-decoration: none;
    color: $m_dark;
    background-color: $m_backgroundGreen;
    padding: 12px 20px;

}
</style>