<template>
    <div class="blogs clearfix">
        <div class="text">
            <p class="subtitle">Read for more joyment</p>
            <h2 class="title">Latest From <span>Our Blogs</span></h2>
        </div>
        <div class="cards">
            <div class="card">
                <img src="../assets/images/artist-blog-03-480x325.jpeg" alt="Old man painting">
                <p class="subtitle">Artist</p>
                <h3>Brush Strokes Energize Trees in Paintings</h3>
                <div class="info">
                    <p><i class="far fa-calendar"></i> May 15, 2020</p>
                    <p><i class="far fa-eye"></i>688 views</p>
                </div>
            </div>
            <div class="card">
                <img src="../assets/images/artist-blog-01-480x325.jpg" alt="Yung girl painting">
                <p class="subtitle">Artist</p>
                <h3>Pocket-Sized Notebooks Hold Miniature Paintings</h3>
                <div class="info">
                    <p><i class="far fa-calendar"></i> May 15, 2020</p>
                    <p><i class="far fa-eye"></i>603 views</p>
                </div>

            </div>
            <div class="card">
                <img src="../assets/images/artist-blog-02-480x325.jpg" alt="Yung boy staring">
                <p class="subtitle">Artist</p>
                <h3>Connection Between Self-Portraits and Identity</h3>
                <div class="info">
                    <p><i class="far fa-calendar"></i> May 15, 2020</p>
                    <p><i class="far fa-eye"></i>397 views</p>
                </div>
            </div>
        </div>
        

    </div>
</template>

<script>
export default {
    name: 'Blogs'
}
</script>

<style lang="scss" scoped>
 @import '~@fortawesome/fontawesome-free/css/all.min.css';
 @import "~@fontsource/poppins/400.css";
 @import "~@fontsource/poppins/600.css";
 @import "~@fontsource/poppins/800.css";
 @import "../style/common.scss";


    @include clearfix;
    .blogs {
        padding: 100px 0;
        text-align: center;
        background-color: #f8f8f8;
        font-family: poppins;
    }
    .text {
        @include text_rules;
    }
    .cards {
        width: 65%;
        margin: auto;
    }
    .card {
        float: left;
        width: 30%;
        height: 300px;
        margin: 40px 10px;
        border-radius: 5px;
        text-align: left;
        background-size: contain;
        background-repeat: no-repeat;

        img {
            width: 100%;
        }
        .subtitle {
            margin: 15px 0 0 0;
            text-transform: uppercase;
            font-size: 12px;
            letter-spacing: 1px;
            color: #706c69;
        }
        h3 {
            font-size: 17px;
            font-weight: 600;
            margin-bottom: 20px
        }
        .info {
            @include infos;
            color: #7e7e7e;
        }

        // &:first-of-type {
        //     background-image: url('../assets/images/artist-blog-03-480x325.jpeg');
        // }
        // &:nth-child(2) {
        //     background-image: url('../assets/images/artist-blog-01-480x325.jpg');
        // }
        // &:nth-child(3) {
        //     background-image: url('../assets/images/artist-blog-02-480x325.jpg');
        // }
    }


</style>