<template>
  <li class="card album">

      <figure class="cardThumb">
          <img :src="album.poster" alt="">
      </figure>

      <div class="infoCard">
          <h3>{{ album.title }} </h3>
          <p>{{ album.author }}</p>
          <p>{{ album.year }} </p>

      </div>

  </li>
</template>

<script>
export default {
    props:{
        album:{
            type: Object,
            required: true,
        }
    }

}
</script>

<style scoped lang="scss">

    .album{
        text-align: center;
        background-color:rgba(white,0.1);
        padding:8px;

        
        .infoCard{
               font-size: 15px;

               h3{
                   padding: 10px;
               }

               p{
                   color: rgba(white,0.2);
                   
               }
               

           }
        
    }

</style>