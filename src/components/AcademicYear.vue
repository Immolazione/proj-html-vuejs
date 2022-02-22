<template>
<section>
    <div class="container pt-4 d-flex flex-column align-items-center justify-content-center">
        <img class="title-img" src="../assets/img/Clock-and-Bell.png" alt="clock-and-bell">
        <h1>University Year</h1>
        <div class="row mt-5">
            <div class="text-center col-3 offset-3">
                <h3>Demo Classes</h3>
                <p>In the first week, students try to accommodate with the teaching style and choose their optional courses</p>
            </div>
            <div class="text-center col-3 offset-2">
                <h3>Graduation Day</h3>
                <p>On the day of graduation, all students gather for the cerimony and then network and party among others</p>
            </div>
            <img id="timeline" src="../assets/img/Timeline-Item.png" alt="timeline">
            <div class="text-center col-3 offset-1">
                <h3>Orientation</h3>
                <p>First day of the university year, all students gather for the opening cerimony and then network with others</p>
            </div>
            <div class="text-center col-3 offset-2">
                <h3>Evaluation</h3>
                <p>At the end of a semester, students take a general evaluation test for every subject they're learning</p>
            </div>
        </div>
    </div>
    <UpcomingEvents />
</section>
</template>

<script>
import UpcomingEvents from './UpcomingEvents.vue'
export default {
    name: 'AcademicYear',
    components: {
        UpcomingEvents
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';

section {
    color: $text-color-white1;
    background-color: $bg-color-red1;
    .container {
        h1, h3 {
            font-family: $itim;
        }
        .title-img {
            height: 3rem;
        }
    }
}
</style>