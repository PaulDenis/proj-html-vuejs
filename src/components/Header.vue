<template>
    <header>
        
        <div class="nav_menu">
            <div class="links">
                <ul class="inline_menu">
                    <li>
                        <a href="#">Home</a>
                        <i class="fas fa-chevron-down"></i>
                    </li>
                    <li>
                        <a href="#">Pages</a>
                        <i class="fas fa-chevron-down"></i>
                    </li>
                    <li>
                        <a href="#">Courses</a>
                        <i class="fas fa-chevron-down"></i>
                    </li>
                    <li>
                        <a href="#">Features</a>
                        <i class="fas fa-chevron-down"></i>
                    </li>
                    <li>
                        <a href="#">Blog</a>
                        <i class="fas fa-chevron-down"></i>
                    </li>
                    <li>
                        <a href="#">Shop</a>
                        <i class="fas fa-chevron-down"></i>
                    </li>
                </ul>
            </div>
            <img src="../assets/images/dark-logo.png" alt="MaxCoach logo" class="logo">
            <div class="search">
                <i class="fas fa-shopping-cart"></i>
                <i class="far fa-user-circle"></i>
                <input type="text" placeholder="Search...">
                <i class="fas fa-search"></i>
            </div>
        </div>
      
        <div class="jumbotron">
            <div class="text">
            <h2 class="title">Commence Business</h2>
            <h2 clasS="mentoring">Distant Mentoring Program</h2>
            <div class="button">
                <p>Download free guidebook</p> 
            </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style lang="scss" scoped>
 @import '~@fortawesome/fontawesome-free/css/all.min.css';
 @import "~@fontsource/roboto";


    .nav_menu {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        display: flex;
        padding: 0 7%;
        // justify-content: space-between;
        align-items: center;
        height: 60px;
        background-color: white;

        .logo {
            height: 20px;
            margin-right: 280px;
        }
        .inline_menu {
            list-style: none;
            margin-right: 80px;
            
            li {
                display: inline-block;
                margin: 0 15px;
                
                a {
                    text-decoration: none;
                    color: black;
                    font-weight: 200;
                    font-size: 14px;
                    padding: 0 5px;
                }
                i {
                    font-size: 8px;
                }
            }
        }
        .search {
            width: 25%;
            i {
                margin: 0 10px;
            }
            input {
                border: none;
                padding: 10px 60px 10px 10px;
                border-radius: 5px;
                background-color: #f5f5f5;
            }
            .fa-search {
                position: relative;
                left: -35px;
                font-size: 12px;
                color: #36af96;
            }
        }
    }

    .jumbotron {
        position: relative;
        height: 550px;
        margin-top: 60px;
        background-image: url('../assets/images/home-3-hero-bg.jpg');
        background-size: contain;
        
        .text {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: white;
            .title {
                font-size: 28px;
                font-weight: 700;
            }
        }
    }

</style>