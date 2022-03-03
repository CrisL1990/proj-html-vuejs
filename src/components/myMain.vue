<template>
    <main>
        <myJumbotron />
        <logoStrip />
        <cloudBased />
        <specialityServices />
    </main>
</template>

<script>

import myJumbotron from './partials/myJumbotron.vue'
import logoStrip from './partials/logoStrip.vue'
import cloudBased from './partials/cloudBased.vue'
import specialityServices from './partials/specialityServices.vue'
export default {

    name: 'myMain',

    components:{
        myJumbotron,
        logoStrip,
        cloudBased,
        specialityServices
    }

}
</script>

<style scoped lang="scss">
    
</style>    