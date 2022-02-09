<template>
<div>
    <SecMainNumb/>
    <SecMainService/>
    <sec-team-main/>
</div>
</template>

<script>
import SecMainNumb from '../section/SecMainNumb.vue'
import SecMainService from '../section/SecMainService.vue'
import SecTeamMain from '../section/SecTeamMain.vue'
export default {
    name: "Main",
    components:{
        SecMainNumb,
        SecMainService,
        SecTeamMain
    }
}
</script>

<style lang="scss" scoped>

</style>


