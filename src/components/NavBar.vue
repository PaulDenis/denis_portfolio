<template>
    <!-- Una normale barra di navigazione, non troppo complessa in quanto si baserà principalmente sulla home -->
    <div  class="inline_menu">
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Projects</a></li>
            <li><a href="#">About me</a></li>
            <li><a href="#">Gallery</a></li>
        </ul>
        <div class="lingue">
            <img v-if="current == ''" v-on:click="lingue = !lingue"
            src="../assets/us.svg" alt="american english" class="flags">
            <img v-else v-on:click="lingue = !lingue"
            :src="current.url" :alt="current.lingua" class="flags">
            <i class="fas fa-chevron-down"  v-on:click="lingue = !lingue"></i>
            <div class="container_lingue"
            v-if="lingue==true">
                <img v-for="flag in flags" :key="flag.url" 
                :src="flag.url" :alt="flag.lingua"
                v-on:click="lingua = flag.lingua, lingue=false, changeLenguage(), $emit('lingua', lingua)"
                class="flags">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'NavBar',
    data() {
        return {
            lingua: 'american english',
            lingue: false,
            flags: [ 
                {
                    lingua:'american english',
                    url: require('../assets/us.svg'),
                },
                {
                    lingua: 'italian',
                    url: require('../assets/it.svg'),
                },
                {
                    lingua:'romanian',
                    url: require('../assets/ro.svg'),
                },
            ],
            current: ""
        }
    },
    methods: {
        changeLenguage: function() {
            for(var i=0; i<this.flags.length; i++) {
                if (this.flags[i].lingua == this.lingua) {
                    // console.log(this.flags);
                    return this.current= this.flags[i];
                }
            }
        }
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/common.scss';

    .inline_menu {
        position: fixed;
        top: 0;
        z-index: 10;
        display: flex;
        justify-content: space-between;
        width: 100%;
        height: 35px;
        background-color: $opposite_color;
        // background-image: linear-gradient(to right, $opposite_color, white);
        ul {
            list-style: none;
            display: flex;
            align-items: center;
            padding: 0;
            height: 100%;
            li {
                display: inline-block;
                padding-right: 30px;
                padding-left: 30px;
                border-right: 1px solid black;
                &:last-child {
                    border: none;
                }
                a {
                    color: black;
                    text-decoration: none;
                    font-weight: 700;
                    &:hover {
                        text-decoration: underline;
                    }
                }
            }
        }
    }
    .lingue {
        margin-right: 50px;
        .flags {
            height: 20px;
            width: 20px;
            &:hover {
                cursor: pointer;
            }
        }
        .fa-chevron-down {
            position: relative;
            top: 3px;
            margin-left: 10px;
            &:hover {
                cursor: pointer;
            }
        }
    }
    .container_lingue {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 30px;
        padding-top: 5px;
        padding-bottom: 5px;
        position: absolute;
        right: 70px;
        top: 30px;
        background-color: $opposite_color;
    }

</style>