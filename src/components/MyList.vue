<template>
 
    <ul>
        <MyAlbum v-for="(album,i) in albums" :key="i" :album="album">
            {{ album.title }}
        </MyAlbum>
    </ul>

</template>

<script>
import axios from 'axios'
import MyAlbum from './MyAlbum.vue'

export default {
    components:{
        MyAlbum,
    },
    data(){
        return {
            albums:[]
        }
    },
    methods:{
        fetchAlbums: function(){

            // chiamata server 
            axios.get(' https://flynn.boolean.careers/exercises/api/array/music')
            .then( res=> {
                this.albums = res.data.response
            })
           .catch ( err => {
               console.erul( err.response);
               this.albums = [ ]
           } )

            // salvare array di album dentro this.album

        }

    },
    created(){
        this.fetchAlbums()
    },

}
</script>

<style scoped lang="scss">

</style>