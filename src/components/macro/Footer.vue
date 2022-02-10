<template>
    <div>
        <sec-mess-top-footer/>
        <middle-footer/>
        <bottom-footer/>
    </div>
</template>

<script>
import BottomFooter from '../section/BottomFooter.vue'
import MiddleFooter from '../section/MiddleFooter.vue'
import SecMessTopFooter from '../section/SecMessTopFooter.vue'
export default {
    name: "Footer",
    components:{
        SecMessTopFooter,
        MiddleFooter,
        BottomFooter
    }
}
</script>

<style lang="scss" scoped>

</style>