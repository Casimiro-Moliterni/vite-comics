<script>
 export default {
    name:'AppFooter',
    data(){
      return{
        images:[
          {
            img:'footer-facebook.png',
          },
          {
            img:'footer-periscope.png',
          },
          {
            img:'footer-pinterest.png',
          },
          {
            img:'footer-twitter.png',
          },
          {
            img:'footer-youtube.png'
          },
        ]
      }
    },
    methods:{
      getImageUrl(name) {
                return new URL(`../assets/img/${name}`, import.meta.url).href;
            }
    }
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
    <div class="footer-bottom">
      <div class="container">
           <button >SIGN-UP-NOW!</button>
           <div class="links-footer-bottom-contain">
                <h2>FOLLW US</h2>
                <img v-for="image in images" :src="getImageUrl(image.img)" alt="">
           </div>
      </div>
    </div>
 </footer>
</template>

<style scoped lang="scss">
@use '../style/partials/-variables' as *;

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
          padding-top: 35px ;
          padding-bottom: 50px;
          text-wrap: nowrap;
          .col{
            width: calc((100% / 3) - 55px);
             h3{
              color: white;
              margin-bottom: 16px;
             }
            li{
              margin-bottom: 7px;
              text-align: left;
              a{
              color: #959578;
             font-size: 13px;
            }
            } 
           .p{
            padding-top: 15px;
           }
          }

         }
    }
  }
  .footer-bottom{
      background-color: #303030;
      padding: 30px 0;

          .container{
           display: flex;
           align-items: center;

           button{
            border: none;
            background-color: inherit;
            border: 3px solid $brand_primary;
            color: white;
            padding: 15px 12px;
            font-weight: 600;
            font-family: inherit;
           }
           .links-footer-bottom-contain{
            margin-left: auto;
            display: flex;
            align-items: center;
            gap:15px ;
             h2{
               color:$brand_primary;
               padding-right: 18px;
             }

           }
         }
  }
</style>