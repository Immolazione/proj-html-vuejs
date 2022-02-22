<template>
  <section class="position-relative">
    <div class="container">
        <div class="row">
            <div class="col-6 d-flex flex-column">
                <img class="mb-4" src="../assets/img/Books-icon.png" alt="books_icon">
                <h1 class="mb-4">Thousands of courses for any type of student</h1>
                <p class="mb-5">At EduPrime, it doesn't matter what domain you wish to purse a career in. Here you can find a course that satisfies your needs within a click away and applies for a course in a matter of minutes. EduPrime is ranked as the most versatile university in the world, thanks to the number of courses it provides.</p>
                <button class="button">Browse throught courses</button>
            </div>
            <div class="col-4 offset-1 d-flex align-items-center justify-content-center"><img src="../assets/img/Graduation-Illustration.png"></div>
        </div>
    </div>
    <img src="../assets/img/home-background.png" class="position-absolute w-100" alt="home_background">
  </section>
</template>

<script>
export default {
    name: 'CoursesSection'
}
</script>

<style scoped lang="scss">
@import '../assets/scss/style.scss';

section {
    height: 600px;
    .container{
        position: relative;
        z-index: 1;
    }
    img {
        top: -30px;
        z-index: 0;
    }
}

.row {
    margin-top: 5rem;
}
.col-6{
    img {
        width: 4rem;
    }
    h1 {
        font-family: $itim;
    }
    button {
        font-family: $itim;
        background-color: $bg-color-yellow;
        color: $text-color-white1;
        border: none;
        padding: 1rem 2rem;
        border-radius: 50px;
        width: 50%;
    }
}
.col-4{
    img {
        height: 20rem;
    }
}

.button:hover{
    background-color: $bg-color-red1;
}

</style>