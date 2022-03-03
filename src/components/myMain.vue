<template>
    <main>
        <myJumbotron />
        <logoStrip />
        <cloudBased />
    </main>
</template>

<script>

import myJumbotron from './partials/myJumbotron.vue'
import logoStrip from './partials/logoStrip.vue'
import cloudBased from './partials/cloudBased.vue'
export default {

    name: 'myMain',

    components:{
        myJumbotron,
        logoStrip,
        cloudBased
    }

}
</script>

<style scoped lang="scss">
    
</style>    