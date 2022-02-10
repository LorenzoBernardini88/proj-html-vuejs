<template>
    <div>
        <sec-mess-top-footer/>
        <middle-footer/>
    </div>
</template>

<script>
import MiddleFooter from '../section/MiddleFooter.vue'
import SecMessTopFooter from '../section/SecMessTopFooter.vue'
export default {
    name: "Footer",
    components:{
        SecMessTopFooter,
        MiddleFooter
    }
}
</script>

<style lang="scss" scoped>

</style>