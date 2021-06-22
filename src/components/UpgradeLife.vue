<template>
    <div class="clearfix container">
        <div class="images">
            <img src="..\assets\images\stock-full-hd-11-670x450.jpg" alt="Lady at the phone">
            <img src="..\assets\images\maxcoach-shape-07-150x150.png" alt="Square shape">
            <img src="..\assets\images\maxcoach-shape-05-150x150.png" alt="Exagon shape">
            <img src="..\assets\images\icon-youtube-play.png" alt="Play button">
        </div>

        <div class="text">
            <p class="subtitle">how we work</p>
            <h2 class="title">Upgrade Your Skills <span>Upgrade Your Life</span></h2>
            <p class="mainText">Opening up more opportunities in front of you to get the ticket to more enjoyable door in life. Getting equipped with new skills for new sets of insights into your career. MaxCoach accompany learners in every stage of learning.</p>
            <p class="guide">Download free guidebook <i class="fas fa-long-arrow-alt-right"></i></p>
        </div>
    </div>
</template>

<script>
export default {
    name: "UpgradeLife"
}
</script>

<style lang="scss" scoped>
 @import '~@fortawesome/fontawesome-free/css/all.min.css';
  @import "~@fontsource/poppins/400.css";
 @import "~@fontsource/poppins/600.css";
@import '../style/common.scss';

    .container {
        width: 65%;
        margin: auto;
        margin-bottom: 100px;
        margin-top: 100px;
    }
    .images {
        position: relative;
        float: left;
        width: 60%;
        height: 400px;

        img:nth-child(1) {
            position: absolute;
            width: 550px;
            z-index: 2;
        }
        img:nth-child(2) {
            position: absolute;
            bottom: -55px;
            right: 25px;
            z-index: 1;
        }
        img:nth-child(3) {
            position: absolute;
            top: 50px;
            left: -95px;
            z-index: 1;
        }
        img:nth-child(4) {
            position: absolute;
            top: 50%;
            left: 50%;
            width: 80px;
            transform: translate(-70%, -70%);
            z-index: 3;
            cursor: pointer;
        }
    }
    .text {
        float: right;
        width: 33%;
        padding-top: 35px;
        font-family: poppins;
        @include text_rules;
        .guide {
            display: inline-block;
            font-size: 12px;
            font-weight: 600;
            border-bottom: 1px solid lightgray;

            &:hover {
                cursor: pointer;
                color: $main_color;
            }
        }
    }
    .clearfix::after {
        content: "";
        display: table;
        clear: both;
    }
</style>