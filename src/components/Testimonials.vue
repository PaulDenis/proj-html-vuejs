<template>
    <div class="testimonials clearfix">
        <div class="text">
            <p class="subtitle">Testimonials</p>
            <p class="title">Why Do People <span>*Hearts*</span> Us?</p>
            <p class="mainText">Seeking for verbals of our service quality? Find them here. Everything is transparent and straightforward for your sense of justification.</p>
            <p class="all">view all <i class="fas fa-long-arrow-alt-right"></i></p>
        </div>
        <div class="reviews">
            <div class="review small">
                <h3>The MaxCoach team works really hard to ensure high level of quality</h3>
                <p>I am happy with their arrangement of lessons and subjects. They do a really good job with every session and I coudn't be more happy.</p>
            </div>
            <div class="review">
                <h3>Professional team of specialists and  passionate mentors at reach</h3>
                <p>I need to get a certification for English proficiency and MaxCoach is my best choise. Their tutors are smart and professional when dealing with students.</p>
                <div class="profile">
                    <img src="../assets/images/testimonial-avata-01.jpg" alt="">
                    <p class="name">Madley Pondor</p>
                    <p>/ IT Specialist</p>
                </div>
            </div>
            <div class="review small">
                <div class="profile">
                    <img src="../assets/images/testimonial-avata-02.jpg" alt="">
                    <p class="name">Mina Hollace</p>
                    <p>/ Freelancer</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Testimonials'
}
</script>

<style lang="scss" scoped>

@import "~@fontsource/poppins/200.css";
@import "~@fontsource/poppins/400.css";
 @import "~@fontsource/poppins/600.css";
 @import "~@fontsource/poppins/800.css";
 @import '~@fortawesome/fontawesome-free/css/all.min.css';
 @import "../style/common.scss";

 @include text_rules;
 @include clearfix;

    .testimonials {
        width: 63%;
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
    .reviews {
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 55%;
        height: 650px;
        float: right;
        font-family: poppins;

        .review {
            position: relative;
            z-index: 2;
            // height: 270px;
            padding: 30px;
            // background-color: red;
            border-radius: 5px;
            box-shadow: 0px 0px 50px 10px #e7e7e7;
            background-color: white;

            h3 {
                font-weight: 400;
                font-size: 15px;
                margin-bottom: 10px;
            }
            p {
                font-size: 14px;
                // letter-spacing:  -0.1px;
                line-height: 24px;
                color: #6d6d6d;
                margin-bottom: 20px;
            }
            img {
                float: left;
                width: 60px;
                border-radius: 50%;
            }
        }
        .small {
            position: absolute;
            top: 87px;
            width: 80%;
            margin: auto;
            z-index: 1;
            // box-shadow: none;
            background-color: white;
            opacity: .5;
            h3 {
                font-size: 12px;
                color: grey;
                font-weight: 600;
            }
            p {
                line-height: 18px;
                font-size: 11px;
            }
            &:last-of-type {
                bottom: 200;
                top: 430px;
                img {
                    width: 40px;
                }
                .profile {
                    p {
                        margin-left: 50px;
                        font-size: 8px;
                        &:first-of-type {
                            font-size: 10px;
                        }
                    }

                }
            }
        }
        .profile {
            p {
                margin: 0;
                margin-left: 80px;
                font-size: 10px;
                &:first-of-type {
                    text-transform: uppercase;
                    font-size: 12px;
                    padding-top: 5px;
                    font-weight: 600;
                    color: black;
                }
            }
        }
    }

</style>