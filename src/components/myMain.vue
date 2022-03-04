<template>
    <main>
        <myJumbotron />
        <logoStrip />
        <cloudBased />
        <specialityServices />
        <makingImpact />
    </main>
</template>

<script>

import myJumbotron from './partials/myJumbotron.vue'
import logoStrip from './partials/logoStrip.vue'
import cloudBased from './partials/cloudBased.vue'
import specialityServices from './partials/specialityServices.vue'
import makingImpact from './partials/makingImpact.vue'
export default {

    name: 'myMain',

    components:{
        myJumbotron,
        logoStrip,
        cloudBased,
        specialityServices,
        makingImpact
    }

}
</script>

<style scoped lang="scss">
    
</style>    