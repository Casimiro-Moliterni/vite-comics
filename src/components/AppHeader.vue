<script>
export default {
   name:'AppHeader',
   data(){
    return {
       links:[
        {
            text:'characters',
            active:false
        },
        {
            text:'comics',
            active:true
        },
        {
            text:'movies',
            active:false
        },
        {
            text:'tv',
            active:false
        },
        {
            text:'games',
            active:false
        },
        {
            text:'collectibles',
            active:false
        },
        {
            text:'videos',
            active:false
        },
        {
            text:'fans',
            active:false
        },
        {
            text:'news',
            active:false
        },
        {
            text:'shop',
            active:false
        },
       ]
    }
   }
}
</script>

<template>
  <header>
    <div class="container">
        <div class="row">
            <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <nav>
                <ul>
                    <li :class="{'active': link.active  }"  v-for="link in links" ><a href="#">{{ link.text }}</a></li>
                </ul>
            </nav>
        </div>
    </div>
  </header>
</template>

<style scoped lang="scss">
@use '../style/partials/-variables' as *;
   .container {
        .row {
           
            padding: 15px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            .logo{
                 
               img{
                   height: 80px;
                }
              }
              nav{
                padding-right: 15px;
                ul{
                    display: flex;
                    justify-content: flex-end;
                    gap: 25px;

                    li {
                        position: relative;
                        a{
                            color:#464646 ;
                            
                        }
                       &.active ::before{
                          content: '';
                          width: 100%;
                          position: absolute;
                          height: 4px;
                          bottom: -50px;
                          
                          background-color:$brand_primary ;
                          
                       }
                      &.active{
                        a{
                            color:$brand_primary;
                        }
                      }
                    }
                }
              }

           }

   }
</style>