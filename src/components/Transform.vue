<template>
    <div class="transform clearfix">
        <div class="collage">
            <img src="../assets/images/home-3-team-image.png" alt="Picture Collage" id="collage">
            <img src="../assets/images/maxcoach-shape-01.png" alt="Lines shape">
            <img src="../assets/images/maxcoach-shape-05-150x150.png" alt="Shape">
            <img src="../assets/images/svg-0.svg" alt="Shape">
            <img src="../assets/images/maxcoach-shape-07-150x150.png" alt="">
        </div>

        <div class="text">
            <p class="subtitle">Everything in <span>MaxCoach</span></p>
            <h2 class="title">We're Here To <span>Tranform</span> You!</h2>
            <p class="mainText">As learners, people can enjoy great companiorship from MaxCoach mentors and educators. We can help you develop and grow at your best.</p>
            <div class="btn"><p>Get Free Guide</p></div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Transform'
}
</script>

<style lang="scss" scoped>

@import "~@fontsource/poppins/400.css";
 @import "~@fontsource/poppins/600.css";
 @import "~@fontsource/poppins/800.css";
 @import "../style/common.scss";

    @include clearfix;
    .transform {
        width: 60%;
        margin: auto;
        font-family: poppins;
    }
    .collage {
        position: relative;
        float: left;
        width: 60%;
        height: 600px;

        img:nth-child(2) {
            position: absolute;
            bottom: 200px;
            left: -250px;
        }
        img:nth-child(3) {
            position: absolute;
            top: 120px;
            left: -95px;
            z-index: 2;
        }
        img:nth-child(4) {
            position: absolute;
            top: 70px;
            width: 120px;
            filter: invert(90%) sepia(46%) saturate(329%) hue-rotate(90deg) brightness(90%) contrast(86%);
        } 
        img:nth-child(5) {
            position: absolute;
            bottom: 95px;
            right: 220px;
            width: 140px;
        }
    }
    #collage {
        position: absolute;
        width: 450px;
        z-index: 3;
    }

    .text {
        @include text_rules;
        float: right;
        width: 35%;
        margin-top: 100px;
        margin-right: 40px;
    }
    .btn {
        display: inline-block;
        padding: 15px 50px;
        font-size: 10px;
        font-weight: 600;
        border-radius: 5px;
        background-color: $main_color;
        border: 1px solid $main_color;
        color: white;
        &:hover {
            color: $main_color;
            background-color: white;
            border: 1px solid $main_color;
            cursor: pointer;
        }
    }
</style>