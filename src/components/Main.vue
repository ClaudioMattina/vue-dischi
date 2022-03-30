<template>

    <div id="color-container">
        <div id="main-container">

        <MainElement v-for=" (element, index) in elementList" :key="index"
        :info="element" />

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
         
         width: 100vw;
         display: flex;
         align-items: center;

            #main-container{
        
            width: 70%;
            margin: 0 auto;
            height: 100%;
            display: flex;
            flex-wrap: wrap;
            

        }
    }

       

</style>