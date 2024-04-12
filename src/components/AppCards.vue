<script>
export default {
    name:'AppCards'
}
</script>

<template>
   <section  class="jumbo">
   </section>
   <section class="card-section">
         <div class="container">
            <div class="text-serie">CURRENT SERIES</div>
               <div class="row">

               </div>
         </div>
   </section>
</template>

<style scoped lang="scss">
@use '../style/partials/-variables' as *;
     .jumbo{
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;
        min-height:400px;      

     }

     .card-section{
      height: 130px;
      background-color: #1c1c1c;
         
        .row{
         width: 95%;
         
        }
     }

     .container{
      position: relative;
      .text-serie{ 
            color: white;
            background-color: $brand_primary ;
            padding: 10px 30px;
            font-size: 20px;
            font-weight: 600;
            position: absolute;
            top:0;
            left: 0;
          }
     }
</style>