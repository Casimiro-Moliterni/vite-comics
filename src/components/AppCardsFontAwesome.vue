<script>
export default {
    name:'AppCardsFontAwesome',
    data(){
        return{
            cards:[
                {
                  image:'buy-comics-digital-comics.png',
                  text:'Digital Comics'
                },
                {
                    image:'buy-comics-merchandise.png',
                    text:'DC Power Visa'
                },
                {
                    image:'buy-comics-subscriptions.png',
                    text:'DC Merchandaise'

                },
                {
                    image:'buy-comics-shop-locator.png',
                    text:'Subscription'
                },
                {
                   image:'buy-dc-power-visa.svg',
                  text:'Comic Shop Locator'
                }
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
   <section >
      <div class="container">
          <div class="row">
              <div class="col" v-for="card in cards">
                  <div class="row-card">
                      <div class="logo">
                       <img :src="getImageUrl(card.image)" alt="">
                      </div>
                      <div class="text">
                        {{ card.text }}
                      </div>
                  </div>
            </div>
        </div>
      </div>
   </section>
</template>

<style scoped lang="scss">
@use '../style/partials/-variables' as *;
section{
    width: 100%;
    background-color:$brand_primary;
}
     .container{
        .row{
            display:flex ;
            justify-content: space-between;
            max-width: 92%;
            margin-left: - 35px;
            margin-right: - 35px;
            margin: 0 auto;
            padding: 45px 0;
             .col{
                 width: calc((100% / 5) - 35px);
                 flex: 0 0 auto;
                 cursor: pointer;
                 .row-card{
                    display: flex;
                    align-items: center;
                    gap: 10px;
                    .logo{
                        img{
                            height:50px;
                            object-fit: contain;
                        }
                        
                    }
                    .text{
                        width: 30%;
                        text-wrap: nowrap;
                        color: white;
                        font-family: inherit;
                        text-transform: uppercase;
                    }
                 }
            }
        }
     }
</style>