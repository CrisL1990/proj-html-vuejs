<template>
    <main>
        <myJumbotron />
        <logoStrip />
        <cloudBased />
        <specialityServices />
        <makingImpact />
        <clientFeedback />
        <getInTouch />
    </main>
</template>

<script>

import myJumbotron from '../components/partials/main partials/myJumbotron.vue'
import logoStrip from '../components/partials/main partials/logoStrip.vue'
import cloudBased from '../components/partials/main partials/cloudBased.vue'
import specialityServices from '../components/partials/main partials/specialityServices.vue'
import makingImpact from '../components/partials/main partials/makingImpact.vue'
import clientFeedback from '../components/partials/main partials/clientFeedback.vue'
import getInTouch from '../components/partials/main partials/getInTouch.vue'
export default {

    name: 'myMain',

    components:{
        myJumbotron,
        logoStrip,
        cloudBased,
        specialityServices,
        makingImpact,
        clientFeedback,
        getInTouch
    }

}
</script>

<style scoped lang="scss">
    
</style>    