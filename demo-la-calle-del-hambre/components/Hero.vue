<template>

        <section class="hero">
            <img class="hero__logo" src="../assets/burger_logo2.png" loading="lazy" alt="logo">
            <div class="hero__social-container">
                <div class="hero__icon-container"><img class="hero__social-icons" src="../assets/ig.svg" width="35px" alt="instagram"></div>
                <div class="hero__icon-container"><img class="hero__social-icons" src="../assets/fb.svg" width="35px" alt="facebook"></div>
                <div class="hero__icon-container"><img class="hero__social-icons" src="../assets/wa.svg" width="35px" alt="whatsapp"></div>
                <div class="hero__icon-container"><img class="hero__social-icons" src="../assets/phone.svg" alt="phone" width="35px"></div>
            </div>
            <h1 class="hero__title">Hamburguesas Burger Park</h1>
            <p class="hero__description">Nuestra especialidad son las hamburguesa a la parrilla</p>
            <p class="hero__hours">Horario: Lunes a Viernes 19 a 23 | Sabados y Domingos 17 a 00</p>
            <p class="hero__contact">Contacto: <a href="tel:221123456">221-123456</a> | <a href="tel:221456789">221-456789</a></p>

    <!-- Categories should be rendered dynamically -->
            <div class="hero-category__container">
                <CategoryButton buttonText="Hamburguesas" href="#hamburguesas"></CategoryButton>
                <CategoryButton buttonText="Milanesas" href="#milanesas"></CategoryButton>
                <CategoryButton buttonText="Ensaladas" href="#ensaladas"></CategoryButton>
                <CategoryButton buttonText="Bebidas" href="#bebidas"></CategoryButton>
                <CategoryButton buttonText="Hamburguesas" href="#hamburguesas"></CategoryButton>
                <CategoryButton buttonText="Milanesas" href="#milanesas"></CategoryButton>
                <CategoryButton buttonText="Ensaladas" href="#ensaladas"></CategoryButton>
                <CategoryButton buttonText="Bebidas" href="#bebidas"></CategoryButton>
            </div>

        </section>
</template>

<script>

export default {
  name: 'Hero',
}
</script>


<style scoped>

.hero {
    text-align: center;
    padding: 4em 2em;
    position: relative;
}

.hero__logo {
    width: 6rem;
    height: auto;
    position: absolute;
    transform: translate(-50%, -110%);
    border-radius: 50px;
}

/*Social Icons*/

.hero__social-container {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
}
.hero__social-icons {
    float: right;
    margin-right: 25px;
    margin-top: 30px;
    margin-bottom: 15px;
}

.hero-category__container {
    display: flex;
    flex-wrap: nowrap;
    justify-content: flex-start;
    gap: 0.5em;
    overflow-x: auto;
    margin: 1.5rem 0;
    -ms-overflow-style: none; /* IE and Edge */
    scrollbar-width: none;    /* Firefox */
}

/*Hide the scrollbar on the category section  */
.hero-category__container::-webkit-scrollbar {
    display:none;
}

/*********************************************/
/*     Media Queries  for smaller screens    */
/*********************************************/

@media screen and (max-width: 34.375rem) {
    .hero__description,
    .hero__hours,
    .hero__contact {
        text-align: left;
    }
}


@media screen and (max-width: 34.375rem) {
       .hero {
            padding: 4rem 1rem;
       } 
    }

/*********************************************/
/*     Media Queries  for smaller screens    */
/*********************************************/
    @media screen and (min-width: 48rem ) {
        .hero-category__container {
        flex-wrap: wrap;
    }
}

    

</style>