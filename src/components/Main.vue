<template>
    <div>
        <WorkCulture/>
        <Stats/>
        <UpgradeLife/>
    </div>
</template>

<script>
import WorkCulture from './WorkCulture.vue'
import Stats from './Stats.vue'
import UpgradeLife from './UpgradeLife.vue'

export default {
    name: "Main",
    components: {
        WorkCulture,
        Stats,
        UpgradeLife
    }

}
</script>

<style lang="scss" scoped>


</style>