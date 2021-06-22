<template>
    <div class="stats">
        <div>
            <p class="numbers">129+</p>
            <p class="text">Enrolled learners</p>
        </div>
        <div>
            <p class="numbers">80</p>
            <p class="text">Finished sessions</p>
        </div>
        <div>
            <p class="numbers">4&#37;</p>
            <p class="text">Satisfaction rate</p>
        </div>
    </div>
</template>

<script>
export default {
    name: "Stats"
}
</script>

<style lang="scss" scoped>
 @import "~@fontsource/roboto/400.css";
 @import "~@fontsource/roboto/500.css";
 @import "~@fontsource/roboto/700.css";

    .stats {
        display: flex;
        justify-content: space-around;
        width: 50%;
        margin: auto;
        margin-bottom: 50px;
        font-family: roboto;
        
        div {
            text-align: center;

            .numbers {
                margin-bottom: 10px;
                font-size: 40px;
                font-weight: 700;
                color: #20ad96;
            }
            .text {
                color:#706c69;
                font-weight: 500;
                text-transform: uppercase;
                font-size: 12px;
                letter-spacing: 2px;
            }
        }
    }

</style>