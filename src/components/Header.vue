<template>
  <div>

    <div id="my-header">

        <div class="my-select">
            <select name="generi" id="">
                <option v-for="(element, index) in elementList " :key="index" value="">{{ element.genre }}</option>
             </select>
        </div>

    </div>

    <Main />
  </div>
  



</template>

<script>

import Main from './Main.vue'
/* import axios from "axios"; */

export default {
    name:"HeaderIndex",
    components:{
        Main
    },

    data: function() {
        return{
            elementList : null,
            
        }
    },

    methods:{
        apiInfo(){
            axios.get('https://flynn.boolean.careers/exercises/api/array/music').then((result) =>{
                this.elementList = result.data.response
                console.log(result.data.response)
            })
        },

        
    }
}
</script>

<style lang="scss" scoped>
    #my-header{
        background-color: grey;
        height: 10vh;
        margin: 0;
        display: flex;
        align-items: center;
        justify-content: center;
    }
</style>