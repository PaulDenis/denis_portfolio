<template>
    <div class="content">
        <Job :lingua="lingua"/>
        <Youtube :lingua="lingua"/>
        <Preset 
        :lingua="lingua"

        />
    </div>
</template>

<script>
import Job from './Job.vue'
import Youtube from './Youtube.vue'
import Preset from './Preset.vue'

export default {
    name: 'Content',
    components: {
        Job,
        Youtube,
        Preset
    },
    props: {
        lingua: String
    },
    data() {
        return {
            
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';


</style>