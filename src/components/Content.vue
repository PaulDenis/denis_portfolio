<template>
    <div class="content">
        <Job />
    </div>
</template>

<script>
import Job from './Job.vue'

export default {
    name: 'Content',
    components: {
        Job
    }
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';


</style>