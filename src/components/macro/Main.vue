<template>
<div>
    <SecMainNumb/>
    <SecMainService/>
</div>
</template>

<script>
import SecMainNumb from '../section/SecMainNumb.vue'
import SecMainService from '../section/SecMainService.vue'
export default {
    name: "Main",
    components:{
        SecMainNumb,
        SecMainService
    }
}
</script>

<style lang="scss" scoped>

</style>