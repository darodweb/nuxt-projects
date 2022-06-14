<template>


      <div>
        <Header />

        <div class="page-wrapper">

          <Hero />

        </div>
      </div>



</template>

<script>
export default {
    name: "IndexPage",
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');

.page-wrapper {
    max-width: 53rem;
    margin-inline: auto;
    background-color: #f8fafc;
    border-bottom-left-radius: 0.375rem;
    border-bottom-right-radius: 0.375rem;
}

:root {
    --main-bg: #F2F5FA;
    --main-headings: #100423;
    --body-text-color: #585065;
    --secondary-color: #E7B65E;
    --btn-bg: white;
    --body-text-size: 0.875rem;
    --body-text-fw: 400;
    --main-headings-size: 1.125rem;
    --main-headings-fw: 400;
    --card-bg: white;
}

/**************************/
/*     General Styles     */
/**************************/
body,
html {
    width: 100%;
	height: 100%;
	background-color: var(--main-bg);
    box-sizing: border-box;
    margin: 0;
    scroll-behavior: smooth;
    overflow-x: hidden;
}

body {
    background: url("https://res.cloudinary.com/foodiewebdev/image/upload/v1643224595/background_pxgvk2.webp") center center no-repeat;
}

p,
a,
a:active,
a:link {
    font-family: 'Lato', sans-serif;
    color: var(--body-text-color);
    font-size: var(--body-text-size);
    line-height: 1.5;
}

h1 {
    font-family: 'Lato', sans-serif;
    color: var(--main-headings);
    font-size: var(--main-headings-size);
}

h2 {
    font-family: 'Lato', sans-serif;
    color: var(--main-headings);
    font-size: var(--main-headings-size);
    line-height: 1.5;
}

/**************************/
/*     Utility classes    */
/**************************/

a.hero-category__item, 
a:link.hero-category__item, 
a:active.hero-category__item {
    outline: var(--secondary-color);
    background-color: var(--btn-bg);
    background-color: var(--btn-bg);
    padding: 10px 15px;
    border: 1px solid var(--secondary-color);
    margin: 3px;
    width: 82px;
    font-weight: 500;
    text-decoration: none;
    border-radius: 5px;
}



</style>
