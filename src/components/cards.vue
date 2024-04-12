<script> 
export default {
    name:'cards',
    props:['image','title']
}
</script>

<template>
 <div class="cards">
    <div class="img">
         <img :src="image" alt="">
    </div>
    <h4>{{title}}</h4>
 </div>
</template>

<style scoped lang="scss"> 
 .cards{
    width: calc((100% / 6) - 12px);
    margin: 12px 0;
    padding: 10px;


     .img{
        width: 180px;
        height: 185px;
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
     }
      
    h4{
        text-align: left;
        font-family: inherit;
        margin-top: 14px;
        font-weight: 400;
        text-transform: uppercase;
    }
    cursor: pointer;
 }

</style>