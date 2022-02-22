<template>
<section class="mt-5 pb-5 position-relative">
    <div id="faculties-title" class="container d-flex flex-column justify-content-center align-items-center">
        <img src="../assets/img/upcoming-events-calendar-icon.png" alt="faculties-logo">
      <h1>Faculties available at EduPrime</h1>
      <p class="text-center">A single university with a load of courses, tailored to satisfy any student's needs.</p>
    </div>
    <div id="event-card" class="mt-5 container d-flex justify-content-between">
        <div
        v-for="(item, index) in coachingSessions"
        :key="index" 
        class="event-card d-flex flex-column align-items-center justify-content-center position-relative pb-2">
            <h2>{{ item.title }}</h2>
            <p class="text-muted text-center">{{ item.date }}</p>
            <p class="text-muted w-75 text-center">{{ item.description }}</p>
            <button class="position-absolute">Find More</button>
        </div>
    </div>
    <div class="other-courses-btn d-flex justify-content-center">
    <button class="button">View All Events</button>
    </div>
</section>
</template>

<script>
export default {
    name: 'UpcomingEvents',
    props: ['coachingSessions']
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';

section{
    img {
        height: 3rem;
    }
    h1, h3{
        font-family: $itim;
    }
    .event-card{
        h2 {
            font-family: $itim;
        }
        color: $text-black7;
        background-color: $bg-color-white1;
        height: 15rem;
        width: calc(100% / 3 - 2rem);
        border-radius: 30px;
    }
}
section > .other-courses-btn button {
    font-family: $itim;
    background-color: $bg-color-yellow;
    color: $text-color-white1;
    border: none;
    margin-top: 4rem;
    padding: 1.5rem 2.5rem;
    border-radius: 50px;
    width: 15%;
}
#event-card{
    button{
        font-family: $itim;
        top: 100%;
        left: 50%;
        transform: translate(-50%, -50%);
        border: none;
        background-color: $bg-color-red1;
        color: $text-color-white1;
        padding: 0.5rem 1rem;
        border-radius: 30px;
        box-shadow: 0 0 5px 0 $border-color-grey4;
    }
}
.button:hover{
    background-color: $bg-color-red2;
}
</style>