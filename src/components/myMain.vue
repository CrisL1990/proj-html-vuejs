<template>
    <main>
        <myJumbotron />
        <logoStrip />
        <cloudBased />
        <specialityServices />
        <makingImpact />
        <clientFeedback />
    </main>
</template>

<script>

import myJumbotron from './partials/myJumbotron.vue'
import logoStrip from './partials/logoStrip.vue'
import cloudBased from './partials/cloudBased.vue'
import specialityServices from './partials/specialityServices.vue'
import makingImpact from './partials/makingImpact.vue'
import clientFeedback from './partials/clientFeedback.vue'
export default {

    name: 'myMain',

    components:{
        myJumbotron,
        logoStrip,
        cloudBased,
        specialityServices,
        makingImpact,
        clientFeedback
    }

}
</script>

<style scoped lang="scss">
    
</style>    