<template>
<section class="position-relative mb-5">
    <div class="d-flex flex-column mt-5 mb-4 container">
        <h1 class="mb-5 text-center">Partners</h1>
        <p class="mb-5 text-center">Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy.</p>
        <div class="d-flex">
            <img v-for="(item, index) in partners" :key="index" class="partner-logo" :src="require(`../assets/img/${item.image}`)" alt="item.alt">
        </div>
    </div>
    <!-- <img class="position-absolute w-100" src="../assets/img/background-wave3.png" alt="wave"> -->
</section>
</template>

<script>
export default {
    name: 'Partners',
    props: ['partners']
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';

section {
    h1 {
        font-family: $itim;
    }
    div{
        .partner-logo {
            height: 4rem;
            margin: 0 5px;
        }
    }
}
</style>