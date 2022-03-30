<template>

    <div id="color-container">
        <div id="main-container">

        <MainElement v-for=" (element, index) in elementList" :key="index"
        :oggetto="ciao" />

  </div>
    </div>
  
</template>

<script>

import axios from "axios";
import MainElement from './MainElement.vue'

export default {
    name:"MainIndex",
    components: {
        MainElement
    },

    data: function() {
        return{
            elementList : null,
        }
    },

    created: function(){
        this.apiInfo()
    },

    methods:{
        apiInfo(){
            axios.get('https://flynn.boolean.careers/exercises/api/array/music').then((result) =>{
                this.elementList = result.data.response
                console.log(result.data.response)
            })
        }
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