<template>

  <div class="my-scheda-container">
      <div class="img-container">
          <img :src="info.poster" alt="">
      </div>
     
      <div class="info-container">
          <h5> {{ info.title }} </h5>
          <p>{{ info.author }}</p>
          <p>{{ info.year }}</p>
      </div>
  </div>

</template>

<script>
export default {
    name:"ElementIndex",
    props: {"info" : Object}
}
</script>

<style lang="scss" scoped>
    .my-scheda-container{
        background-color: rgb(36, 36, 41);
        width: calc(90% / 5);
        height: 400px;
        margin: 20px 1%;
        display: flex;
        flex-direction: column;
        justify-content: space-around;

        .img-container{
            height: calc(70% - 20%);
            padding: 10%;
        }
        img{
            width: 100%;
            height: 100%;
        }
        
        

            .info-container{
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                color: lightgreen;
                height: 30%;
                


                    h5{
                        color: white;
                        font-size: .4;
                    }
            }

            
    }
</style>