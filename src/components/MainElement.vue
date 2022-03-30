<template>
  <div class="my-scheda-container">
     <img src="" alt="">
      <div class="info-container">
          <h2> {{elementList.title}} </h2>
          <p>Ciao</p>
          <p>1995</p>
      </div>
  </div>
</template>

<script>
export default {
    name:"ElementIndex",
    props: {"ciao" : Object}
}
</script>

<style lang="scss" scoped>
    .my-scheda-container{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border: 1px solid white;
        width: calc(100% / 5); 
        background-color: rgb(36, 36, 41);

            .info-container{
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                color: lightgreen;

                    h2{
                        color: white;
                    }
            }

            
    }
</style>