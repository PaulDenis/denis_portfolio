<template>
    <div class="content">
        <Job :lingua="lingua"/>
        <Youtube :lingua="lingua"/>
    </div>
</template>

<script>
import Job from './Job.vue'
import Youtube from './Youtube.vue'

export default {
    name: 'Content',
    components: {
        Job,
        Youtube
    },
    props: {
        lingua: String
    }
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';


</style>