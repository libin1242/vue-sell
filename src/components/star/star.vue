<template>
    <div class="star" :class="starType">
        <span v-for="itemClass in itemClass" :class="itemClass" class="stat-item"></span>
    </div>
</template>
<script type="text/ecmascript-6">
export default {
    props: {
        size: {
            type: Number
        },
        score: {
            type: Number
        }
    },
    computed: {
        starType() {
            return 'star-' + this.size;
        }
    }
};
</script>

<style lang="stylus" rel="stylesheet/stylus">
.star
    font-size 0
    .star-item
        display inline-block
    &.star-48
    &.star-36
    &.star-24
        
 
</style>

