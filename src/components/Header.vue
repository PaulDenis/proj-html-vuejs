<template>
    <header>
        
        <div class="nav_menu">
            <div class="links">
                <ul class="inline_menu">
                    <li v-for="(link,index) in links" :key="index">
                        <a href="#">{{ link }}</a>
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
                <i class="fas fa-long-arrow-alt-right"></i>
            </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    props: {
        links: Array
    }
}
</script>

<style lang="scss" scoped>
 @import '~@fortawesome/fontawesome-free/css/all.min.css';
 @import "~@fontsource/poppins/200.css";
 @import "~@fontsource/poppins/400.css";
 @import "~@fontsource/poppins/600.css";
 @import "~@fontsource/poppins/700.css";
 @import "~@fontsource/poppins/800.css";




    .nav_menu {
        position: fixed;
        top: 0;
        left: 0;
        z-index: 5;
        width: 100%;
        display: flex;
        padding: 0 7%;
        // justify-content: space-between;
        align-items: center;
        font-family: poppins;
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
                margin: 0 10px;
                
                a {
                    text-decoration: none;
                    color: black;
                    font-weight: 400;
                    font-size: 12px;
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
        background-size: cover;
        
        .text {
            display: flex;
            flex-direction: column;
            align-items: center;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-family: poppins;
            color: white;
            .title {
                font-size: 28px;
                font-weight: 600;
                margin: 5px;
            }
            .mentoring {
                font-size: 46px;
                font-weight: 400;
                line-height: 46px;
            }
            .button {
                width: 250px;
                padding: 15px;
                margin-top: 25px;
                border-radius: 5px;
                text-align: center;
                font-size: 10px;
                font-weight: 800;
                background-color: white;
                color: #36af96;
                p {
                    display: inline-block;
                    margin-right: 10px;
                }
                i {
                    font-size: 12px;
                }
                &:hover {
                    cursor: pointer;
                    color: white;
                    background-color: #36af96;
                }
            }
        }
    }

</style>