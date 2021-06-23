<template>
  <footer>
    <div class="links">

        <div>
            <h2 class="title">Address</h2>
            <p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
            <p>+1(305)547-9909 (9am - 5pm EST, Monday - Friday</p>
            <p>support@maxcoach.com</p>
            <div id="social">
                <ul>
                    <li><i class="fab fa-facebook-square"></i></li>
                    <li><i class="fab fa-twitter"></i></li>
                    <li><i class="fab fa-instagram"></i></li>
                    <li><i class="fab fa-linkedin"></i></li>
                </ul>
            </div>
        </div>
        <div class="explore">
            <h2 class="title">Explore</h2>
            <ul>
                <li
                v-for="(link, index) in explore" :key="index">
                <p>{{link}}</p>
                </li>
            </ul>
        </div>
        <div class="informations">
            <h2 class="title">Information</h2>
            <ul>
                <li v-for="(info, index) in informations" :key="index">
                    <p>{{ info }}</p>
                </li>
            </ul>
        </div>
      </div>
      <div class="copy">
          <p>&copy; 2020 Maxcoach. All Rights Reserved</p>
      </div>
  </footer>
</template>

<script>
export default {
    name: "Footer",
    props: {
        explore: Array,
        informations: Array
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

    footer {
        // height: 500px;
        background-color: #171621;
        text-align: center;
        font-family: poppins;
        font-weight: 600;
        color: #9da4a0;

    }
    .links {
        display: flex;
        width: 75%;
        padding-top: 50px;
        margin: auto;
        justify-content: space-around;
        text-align: left;

        ul {
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            height: 120px;
            list-style: none;
            li {
                margin-right: 50px;
            }
        }
        .explore {
            ul {
                height: 140px;
                li {
                    width: 70px;
                }

            }
        }
        .informations {
            ul {
                height: 170px;
                li {
                    width: 90px;
                }
            }
        }
        div {
            display: inline-block;
            // margin-right: 70px;
        }
        .title {
            font-size: 14px;
            color: white;
        }
        p {
            margin: 10px 0;
            font-size: 10px;
            &:hover {
            cursor: pointer;
            text-decoration: underline;
            }
        }
        
    }
    #social {
        margin-left: 0;
        margin-top: 20px;
        ul {
            display: flex;
            flex-direction: row;
            justify-content: flex-start;
            flex-wrap: nowrap;
            li {
                margin-right: 25px;
                font-size: 20px;
            }
        }
    }
    .copy {
            padding-bottom: 25px;
            font-size: 10px;
        }
</style>