<template>
  <div class="my-scheda-container">
     
      <div class="info-container">
          <h2>CIAO</h2>
          <p>Ciao</p>
          <p>1995</p>
      </div>
  </div>
</template>

<script>
export default {
    name:"Element"
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