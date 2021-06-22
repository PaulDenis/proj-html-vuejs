<template>
    <div class="courses">
        <div class="text">
            <p class="subtitle">Join maxcoach at best</p>
            <h2 class="title">Latest Online <span>Courses</span></h2>
        </div>
        <div class="cards clearfix">
            <div class="card">
                <p class="price"><span>$40</span>.00</p>
                <p class="courseTitle">Learning to Write as a Professional Author</p>
                <div class="icons">
                    <p><i class="far fa-file-alt"></i> 20 Lessons</p>
                    <p><i class="far fa-user"></i> 50 Students</p>
                </div>
            </div>
            <div class="card">
                <p class="price"><span>$0</span>.00</p>
                <p class="courseTitle">Custumer-centric Info-Tech Strategies</p>
                <div class="icons">
                    <p><i class="far fa-file-alt"></i> 24 Lessons</p>
                    <p><i class="far fa-user"></i> 769 Students</p>
                </div>
            </div>
            <div class="card">
                <p class="price"><span>$19</span>.00</p>
                <p class="courseTitle">Open programming Courses for Everyone: Python</p>
                <div class="icons">
                    <p><i class="far fa-file-alt"></i> 17 Lessons</p>
                    <p><i class="far fa-user"></i> 62 Students</p>
                </div>
            </div>
        </div>
        <div class="circles">
            <i class="fas fa-circle active"></i>
            <i class="fas fa-circle"></i>
            <i class="fas fa-circle"></i>
            <i class="fas fa-circle"></i>
            <i class="fas fa-circle"></i>
        </div>
        <div class="bottomText">
            <p class="courses">Control your personal preference settings to get notified about appropriate courses. <span>View all courses <i class="fas fa-long-arrow-alt-right"></i></span></p>
        </div>
    </div>
</template>

<script>
export default {
    name: "Courses"
}
</script>

<style lang="scss" scoped>
 @import "~@fontsource/poppins/400.css";
 @import "~@fontsource/poppins/600.css";
 @import "~@fontsource/poppins/800.css";
 @import '~@fortawesome/fontawesome-free/css/all.min.css';
 @import "../style/common.scss";

    @include clearfix;
    .text {
        font-family: poppins;
        text-align: center;
        @include text_rules;
    }
    .cards {
        width: 60%;
        margin: auto;
    }
    .card {
        float: left;
        width: 31%;
        margin: 10px;
        border-radius: 5px;
        padding: 20px;
        padding-top: 200px;
        background-size: contain;
        background-repeat: no-repeat;
        background-color: white;
        font-family: poppins;

        .price {
            color: $main_color;
            font-weight: 800;
            font-size: 14px;
            margin-bottom: 5px;
            span {
                font-size: 20px;
            }
        }
        .courseTitle {
            font-weight: 600;
            margin-bottom: 25px;
            color: #4f4f4f;
        }
        .icons {
            display: flex;
            font-size: 10px;
            color: #a8a6b9;
            
            p {
                margin-right: 20px;
                i {
                    margin-right: 5px;
                }
            }
            
        }
        
        img {
            border-radius: 5px;
            width: 100%;
        }
        &:nth-child(1) {
            background-image: url("../assets/images/course-02-480x298.jpg");
        }
        &:nth-child(2) {
            background-image: url('../assets/images/stock-full-hd-03-480x298.jpg');
        }
        &:nth-child(3) {
           background-image: url('../assets/images/stock-full-hd-04-480x298.jpg');
        }
        &:hover {
            cursor: pointer;
            .courseTitle {
                color: $main_color;
            }
                box-shadow: 2px 5px 10px lightgray;
        }
    }

    .circles {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 10px;
        font-size: 6px;
        color: #d8d8d8;

        i {
            margin: 0 10px;
        }
        .active {
            font-size: 10px;
            color: black;
        }
    }
    .bottomText {
        width: 30%;
        margin: auto;
        padding-bottom: 100px;
        text-align: center;
        font-family: poppins;
        font-size: 14px;
        color: #706c69;


        span {
            font-weight: 600;
            color: black;
            border-bottom: 1px solid #d8d8d8;

            &:hover {
                cursor: pointer;
                color: $main_color;
            }
        }
    }
</style>