<template>
  <footer>
      <div class="links">

        <div>
            <h2 class="title">Address</h2>
            <p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
            <p>+1(305)547-9909 (9am - 5pm EST, Monday - Friday</p>
            <p>support@maxcoach.com</p>
            <div class="social">
                <ul>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
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
        <div>
            <h2 class="title">Information</h2>
            <li v-for="(info, index) in informations" :key="index">
                <p>{{ info}}</p>
            </li>
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
        Informations: Array
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
        // margin-bottom: 20px;
        justify-content: center;
        text-align: left;

        ul {
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            height: 130px;
            list-style: none;
            li {
                margin-right: 50px;
            }
        }
        div {
            margin: 0 100px;
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
    .copy {
            padding-bottom: 25px;
            font-size: 10px;
        }
</style>