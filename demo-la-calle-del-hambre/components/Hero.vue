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

            <div class="hero-category__container">
                <a class="hero-category__item" href="#hamburguesas">Hamburguesas</a>
                <a class="hero-category__item" href="#milanesas">Milanesas</a>
                <a class="hero-category__item" href="#ensaladas">Ensaladas</a>
                <a class="hero-category__item" href="#bebidas">Bebidas</a>
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
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.5em;
}


</style>