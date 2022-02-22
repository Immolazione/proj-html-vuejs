<template>
<section>
    <div id="subscribe" class="container d-flex justify-content-between">
        <h1>Subscribe Now to Our Newsletter!</h1>
        <div class="d-flex position-relative">
            <input class="ps-4" type="text" placeholder="Email address...">
            <div class="position-absolute"></div>
        </div>
    </div>
</section>
</template>

<script>
export default {
    name: 'Subscribve'
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';

section {
    background-color: $bg-color-red1;
    #subscribe{
        padding: 4rem 0;
        h1 {
            font-family: $itim;
            color: $text-color-white1;
        }
        div {
            input {
                border: none;
                width: 30rem;
                border-radius: 30px;
                font-family: $itim;
            }
            div {
                background-color: $bg-color-yellow;
                height: 3.5rem;
                width: 3.5rem;
                border-radius: 50%;
                right: 0;
            }
        }
    }
}
</style>