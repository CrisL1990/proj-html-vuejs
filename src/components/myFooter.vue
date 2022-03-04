<template>
    <footer>
        <footerTop />
        <footerBottom />
    </footer>
</template>

<script>

import footerTop from './partials/footer partials/footerTop.vue'
import footerBottom from './partials/footer partials/footerBottom.vue'
export default {

    name: 'myFooter',

    components:{
        footerTop,
        footerBottom
    }

}
</script>

<style scoped lang="scss">

</style>