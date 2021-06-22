<template>
    <div class="testimonials clearfix">
        <div class="text">
            <p class="subtitle">Testimonials</p>
            <p class="title">Why Do People <span>*Hearts*</span> Us?</p>
            <p class="mainText">Seeking for verbals of our service quality? Find them here. Everything is transparent and straightforward for your sense of justification.</p>
            <p class="all">view all <i class="fas fa-long-arrow-alt-right"></i></p>
        </div>
        <div class="image">

        </div>
    </div>
</template>

<script>
export default {
    name: 'Testimonials'
}
</script>

<style lang="scss" scoped>

@import "~@fontsource/poppins/400.css";
 @import "~@fontsource/poppins/600.css";
 @import "~@fontsource/poppins/800.css";
 @import '~@fortawesome/fontawesome-free/css/all.min.css';
 @import "../style/common.scss";

 @include text_rules;
 @include clearfix;

    .testimonials {
        width: 60%;
        margin: auto;
    }
    .text {
        margin-top: 200px;
        margin-bottom: 50px;
        float: left;
        width: 35%;
        font-family: poppins;
    }
    .all {
        display: inline-block;
        font-size: 12px;
        font-weight: 600;
        border-bottom: 1px solid #a8a6b9;
        &:hover {
            cursor: pointer;
        }
    }

</style>