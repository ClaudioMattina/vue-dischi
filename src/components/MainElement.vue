<template>

  <div class="my-scheda-container">
      <div class="img-container">
          <img src="https://i0.wp.com/rkonair.com/wp-content/uploads/2020/11/ACDC.jpg?fit=1800%2C1200&ssl=1" alt="">
      </div>
     
      <div class="info-container">
          <h2>TITOLO</h2>
          <p>Nome artista</p>
          <p>1995</p>
      </div>
  </div>

</template>

<script>
export default {
    name:"ElementIndex",
    /* props: {"ciao" : Object} */
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


                    h2{
                        color: white;
                    }
            }

            
    }
</style>