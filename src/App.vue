<template>
  <div id="app">

    <!--Inizio Header-->
    <myHeader> 

    </myHeader>
    <!--Fine Header-->

    <!--Inizio Main-->
    <myMain>

    </myMain>
    <!--Fine Main-->

    <!--Inizio Footer-->
    <myFooter>

    </myFooter>
    <!--Fine Footer-->

  </div>
</template>

<script>

import myHeader from './components/myHeader.vue'
import myMain from './components/myHeader.vue'
import myFooter from './components/myFooter.vue'

export default {
  
  components:{
    myHeader,
    myMain,
    myFooter
  }

}
</script>

<style lang="scss">
  @import "./assets/style/common.scss";
</style>
