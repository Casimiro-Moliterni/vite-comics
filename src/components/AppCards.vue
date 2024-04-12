<script>
export default {
    name:'AppCards'
}
</script>

<template>
   <section  class="jumbo">
      <div class="container">
        <div class="text-serie">CURRENT SERIES</div>
      </div>
   </section>
   <section class="card-section">

   </section>
</template>

<style scoped lang="scss">
@use '../style/partials/-variables' as *;
     .jumbo{
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;

        .container{
         position: relative;
        min-height:400px;
          
          .text-serie{ 
            color: white;
            background-color: $brand_primary ;
            padding: 10px 30px;
            font-size: 18px;
            font-weight: 600;
            position: absolute;
            bottom: -20px;
            left: 0;
          }
        }

     }

     .card-section{
      height: 130px;
      background-color: #1c1c1c;
     }
</style>