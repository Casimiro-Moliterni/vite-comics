<script>
export default {
   name:'AppHeader'
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
                    <li><a href="#">characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">Tv</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Collectibles</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">Fans</a></li>
                    <li><a href="#">News</a></li>
                    <li><a href="#">Shop</a></li>
                </ul>
            </nav>
        </div>
    </div>
  </header>
</template>

<style scoped lang="scss">
   .container {

        .row {
            border: 1px solid black;
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
                    gap: 10px;
                }
              }

           }

   }
</style>