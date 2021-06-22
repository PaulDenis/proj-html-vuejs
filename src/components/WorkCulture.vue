<template>
    <div class="work">
        <div class="text">
        <p class="subtitle">everything in <span>maxcoach</span></p>
        <h2 class="title">Learn about our <span>Work Culture</span> at MaxCoach</h2>
        <p class="mainText">Spend some time to visit our website or head office and discover our current courses, enrollment procedure, and registration deadline. We're opening new classes every beginning of each month.</p>
        <p class="guide">Have questions? <span>Get Free Guide <i class="fas fa-long-arrow-alt-right"></i></span></p>
        </div>
        <div class="images">
            <img src="..\assets\images\about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg" alt="Girl with Laptop">
            <img src="../assets/images/maxcoach-shape-02.png" alt="Circle shape">
            <img src="../assets/images/maxcoach-shape-07-100x100.png" alt="Square shape">
            <img src="..\assets\images\stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="Office group">
            <!-- <img src="" alt=""> -->
        </div>
    </div>
</template>

<script>
export default {
    name: "WorkCulture"
}
</script>

<style lang="scss" scoped>
 @import '~@fortawesome/fontawesome-free/css/all.min.css';
 @import "~@fontsource/poppins/200.css";
 @import "~@fontsource/poppins/400.css";
 @import "~@fontsource/poppins/600.css";
 @import "~@fontsource/poppins/700.css";
 @import "~@fontsource/poppins/800.css";

    .work {
        height: 500px;
        width: 65%;
        margin: auto;
        margin-bottom: 50px;
        font-family: poppins;
    }
    .text {
        float: left;
        width: 35%;
        margin-top: 150px;
        .subtitle {
            margin-bottom: 20px;
            text-transform: uppercase;
            font-size: 14px;
            color: #706c69;
            span {
                font-weight: 600;
            }
        }
        .title {
            font-size: 34px;
            font-weight: 600;
            line-height: 40px;
            margin-bottom: 20px;
            span {
                font-weight: 400;
                color: #21ad96;
            }
        }
        .mainText {
            margin-bottom: 25px;
            font-size: 12px;
            color: #706c69;
        }
        .guide {
            font-size: 12px;
            span {
                border-bottom: 1px solid lightgray;
                font-weight: 600;
                color: #21ad96;
                cursor: pointer;
            }
        }
    }
    .images {
        position: relative;
        float: right;
        width: 60%;
        height: 450px;
        padding-top: 100px;
        margin-top: 30px;
        img:first-child {
            position: absolute;
            top: 50px;
            right: -50px;
            z-index: 3;
            width: 150px;
            border-radius: 5px;
        }
        img:nth-child(2) {
            position: absolute;
            bottom: -30px;
            right: 40px;
            z-index: 3;
            width: 100px;
        }
        img:nth-child(3) {
            position: absolute;
            top: 60px;
            right: 40px;
            z-index: 1;
        }
        img:nth-child(4) {
            position: absolute;
            right: 0;
            top: 120px;
            z-index: 2;
            width: 450px;
        }
    }

</style>