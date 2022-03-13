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
        padding:10px;
    }

</style>