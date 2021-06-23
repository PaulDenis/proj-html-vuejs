<template>
    <div>
        <div class="gradient">
            <WorkCulture/>
            <Stats/>
            <UpgradeLife/>
            <Courses/>
        </div>
        <Testimonials/>
        <Transform/>
        <Blogs/>
        <Newsletter/>
        
    </div>
</template>

<script>
import WorkCulture from './WorkCulture.vue'
import Stats from './Stats.vue'
import UpgradeLife from './UpgradeLife.vue'
import Courses from './Courses.vue'
import Testimonials from './Testimonials.vue'
import Transform from './Transform.vue'
import Blogs from './Blogs.vue'
import Newsletter from './Newsletter.vue'

export default {
    name: "Main",
    components: {
        WorkCulture,
        Stats,
        UpgradeLife,
        Courses,
        Testimonials,
        Transform,
        Blogs,
        Newsletter
    }

}
</script>

<style lang="scss" scoped>
    .gradient {
        background-image: linear-gradient(white, #f5f5f5);
        border-bottom-right-radius: 110% 10%;
        border-bottom-left-radius: 110% 10%;

    }

</style>