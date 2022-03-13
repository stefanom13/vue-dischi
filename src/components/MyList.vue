<template>
 
    <section>
        <!-- v-for -->
        
    </section>

</template>

<script>
import axios from 'axios'

export default {
    data(){
        return {
            album:[

            ]
        }
    },
    methods:{
        fetchAlbums: function(){

            // chiamata server 
            axios.get(' https://flynn.boolean.careers/exercises/api/array/music')

            // salvare array di album dentro this.album

        }

    },
    created(){
        this.fetchAlbums()
    },

}
</script>

<style>

</style>