<template>

    <div id="color-container">
        <div id="main-container">

        <MainElement />

  </div>
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

<style lang="scss" scoped>

    #color-container{
         background-color: rgb(19, 19, 20); ;
    }

    #main-container{
        
        height: 90vh;
        width: 60%;
        margin: 0 auto;
        
    }

</style>