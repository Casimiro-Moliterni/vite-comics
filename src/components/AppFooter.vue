<script>
 export default {
    name:'AppFooter'
 }
</script>

<template>
 <footer>
    <div class="footer-top">
        <div class="container">
            <div class="row">
               <div class="col" >
                 <h3>DC COMICS</h3>
                 <ul>
                  <li><a href="#">Characters</a></li>
                  <li><a href="#">Comics</a></li>
                  <li><a href="#">Movies</a></li>
                  <li><a href="#">Tv</a></li>
                  <li><a href="#">Games</a></li>
                  <li><a href="#">Videos</a></li>
                  <li><a href="#">News</a></li>
                 </ul>
                 <h3 class="p">SHOP</h3>
                 <ul>
                  <li><a href="#">Shop DC</a></li>
                  <li><a href="#">Shop DC</a></li>
                 </ul>
               </div>
               <div class="col" >
                 <h3 >DC</h3>
                 <ul>
                  <li><a href="#">Terms Of Use</a></li>
                  <li><a href="#">Privacy policy (New)</a></li>
                  <li><a href="#">Ad Choise</a></li>
                  <li><a href="#">Advertising</a></li>
                  <li><a href="#">Jobs</a></li>
                  <li><a href="#">Subscriptions</a></li>
                  <li><a href="#">Talent WorkShops</a></li>
                  <li><a href="#">CPSC Certicates</a></li>
                  <li><a href="#">Ratings</a></li>
                  <li><a href="#">Shop Help</a></li>
                  <li><a href="#">Contacs Us</a></li>
                 </ul>
               </div>
               <div class="col" >
                 <h3>SITES</h3>
                 <ul>
                  <li><a href="#">DC</a></li>
                  <li><a href="#">MAD Magazine</a></li>
                  <li><a href="#">DC Kids</a></li>
                  <li><a href="#">DC Universe</a></li>
                  <li><a href="#">DC Power Visa</a></li>
                 </ul>
               </div>            
            </div>
        </div>
    </div>
 </footer>
</template>

<style scoped lang="scss">
  .footer-top{
    background-image: url('../assets/img/footer-bg.jpg');


    .container{
        background-image: url('../assets/img/dc-logo-bg.png');
        background-position: 100%;
        background-repeat: no-repeat;
         .row{
          width: 30%;
          height: 100%;
          display: flex;
          justify-content: space-between;
          flex-wrap: wrap;
          padding: 35px 0;
          text-wrap: nowrap;
          .col{
            width: calc((100% / 3) - 55px);
             h3{
              color: white;
              margin-bottom: 18px;
             }
            li{
              margin-bottom: 7px;
              text-align: left;
              a{
              color: #959578;
             font-size: 12px;
            }
            } 
           .p{
            padding-top: 15px;
           }
          }

         }
    }
  }
</style>