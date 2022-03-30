<template>
  <div id="main-container">

      <MainElement />

  </div>
</template>

<script>

import MainElement from './MainElement.vue'

export default {
    name:"MainIndex",
    components: {
        MainElement
    }
}
</script>

<style langh="scss" scoped>

    #main-container{
        background-color: rgb(19, 19, 20);
        height: 90vh;
    }

</style>