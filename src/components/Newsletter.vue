<template>
    <div class="newsletter">
        <div class="form">
            <h2 class="title">Subscribe <span>Newsletters</span></h2>
            <p class="mainText">Enter your email address to register to our newsletter subscription delivered on a regula basis!</p>
            <div class="subscribe">
                <input type="text" placeholder="Enter your email">
                <div class="btn">
                    <p>Subscribe</p>
                </div>
            </div>
        </div>
            <img src="../assets/images/maxcoach-shape-02.png" alt="Shape">
            <img src="../assets/images/maxcoach-shape-09.png" alt="Shape">

    </div>
</template>

<script>
export default {
    name: 'Newsletter'
}
</script>

<style lang="scss" scoped>
@import '~@fortawesome/fontawesome-free/css/all.min.css';
 @import "~@fontsource/poppins/400.css";
 @import "~@fontsource/poppins/600.css";
 @import "~@fontsource/poppins/800.css";
 @import "../style/common.scss";

    @include text_rules;
    .newsletter {
        position: relative;
        font-family: poppins;
        padding: 50px 0;
        margin-bottom: 20px;

        img:nth-of-type(1) {
            position: absolute;
            top: 100px;
            width: 100px;
            right: 300px;
        }
        img:nth-of-type(2) {
            position: absolute;
            top: 25px;
            width: 150px;
            right: 290px;
        }
    }
    .form {
        width: 32%;
        margin: auto;
        text-align: center;

        .mainText {
            font-size: 14px;
            font-weight: 400;
            margin-bottom: 40px;
        }
        .subscribe {
            display: flex;
            width: 100%;
            border-radius: 5px;
            overflow: hidden;
            background-color: #f5f5f5;

            input {
                width: 80%;
                padding: 15px 20px;
                border: none;
                background-color: #f5f5f5;
            }
            .btn {
                width: 20%;
                font-size: 10px;
                font-weight: 600;
                line-height: 45px;
                color: white;
                background-color: $main_color;

                &:hover {
                    cursor: pointer;
                    background-color: rgba($color: $main_color, $alpha: .8);
                }
            }
        }
        
    }
</style>