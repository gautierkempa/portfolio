<template>
    <div>
    <h2> Mes compétences </h2>

    <skills v-bind:skills = "skills" > </skills>

    </div>
</template>

<script>
import skills from '@/pages/index.vue'

export default
{
  components:{
    skills
  },


  data (){
    return{
      skills :[
                {
                  nom : ' Montage vidéo ',
                  

                },

                {
                  nom : ' Graphisme ',

                },

                {
                  nom : ' Développement '

                }
              ],
          }
       }

}

</script>

<style>

</style>