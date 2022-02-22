<template>
<section class="container">
    <div>
        <h1 class="section-title">Latest Courses</h1>
        <div class="d-flex justify-content-between">
            <div 
            v-for="(item, index) in latestCourses" 
            :key="index" 
            class="latest-course-card d-flex flex-column align-items-center justify-content-center pb-2 position-relative">
                <img class="efficient-method-icons" :src="require(`../assets/img/${item.image}`)" :alt="item.title">
                <h1 class="text-center">{{ item.title }}</h1>
                <p>Teacher: <strong>{{ item.teacher }}</strong></p>
                <p>price: <strong>{{ item.price }}</strong></p>
                <button class="position-absolute courses-button">View Course</button>
            </div>
        </div>
    </div>
    <div 
    class="methods-and-fees container" 
    v-for="(data, index) in methodsAndFees" 
    :key="index">
        <div class="row" :class="{'row-reverse': data.rowReverse}">
            <div class="col-6">
                <img class="method-and-fees-icons mt-5" :src="require(`../assets/img/${data.icon}`)" alt="data.title">
                <h1 class="mt-3">{{ data.title }}</h1>
                <p class="mt-5">{{ data.paragraph }}</p>
                <button class="button">{{ data.button }}</button>
            </div>
            <div class="col-6">
                <img class="method-and-fees-imgages" :src="require(`../assets/img/${data.image}`)" :alt="data.title">
            </div>
        </div>
    </div>
</section>
</template>

<script>
export default {
    name: 'LatestCourse',
    props : ['latestCourses', 'methodsAndFees']
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';

section {
    margin: 5rem 0;
    .latest-course-card {
        height: 18rem;
        width: 18rem;
        border-radius: 15px;
        box-shadow: 0 0 2px 0 $border-color-grey4;
    }
    h1 {
        font-family: $itim;
        font-size: 1.4rem;
    }
    .section-title {
        font-size: 3rem;
        margin-bottom: 2rem;
    }
    .method-and-fees-icons, .efficient-method-icons {
        height: 4rem;
    }
    .courses-button{
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
.methods-and-fees{
    margin-top: 8rem;
}
.method-and-fees-imgages {
    height: 30rem;
}

button {
    font-family: $itim;
    background-color: $bg-color-red1;
    color: $text-color-white1;
    border: none;
    padding: 1.5rem 2.5rem;
    border-radius: 50px;
}

.row-reverse {
    display: flex;
    flex-direction: row-reverse;
}
.button:hover{
    background-color: $bg-color-yellow;
}
</style>