<template>
    <button class="category-btn" :href="href">
        {{buttonText}}
    </button>
</template>


<script>
export default {
    name: 'CategoryButton',
    props: {
        href: {
            type: String
        },
        buttonText: {
            type: String
        }
    }
}


</script>

<style scoped>

.category-btn {
    outline: var(--secondary-color);
    outline: var(--secondary-color);
    background-color: white;
    background-color: var(--btn-bg);
    padding: 10px 15px;
    border: 1px solid var(--secondary-color);
    margin: 3px;
    font-weight: 500;
    text-decoration: none;
    border-radius: 5px;
    background-color: var(--secondary-color);
}


</style>
