<template>
    <div class="content">
        <Job />
        <Youtube />
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
    }
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';


</style>