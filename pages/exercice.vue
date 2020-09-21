<template>

<div>
    <h1 class="text-center" > Devis  </h1>
      <devis v-on:choix="option" :total="prix" :detail="commande"  />

</div>


</template>

<script>
import devis from '@/components/devis.vue';

export default {
    data(){
        return{
            prix:0,
            commande : "",
        }
    },
    methods:{
        option(opt){
            if(opt == "creasite"){
                this.prix+= 500;
                this.commande += "Création de site web / "
            }
            if(opt == "graphisme"){
                this.prix+= 200;
                this.commande += "Infographie / "
            }
             if(opt == "montagevideo"){
                this.prix+= 300;
                this.commande += "Montage vidéo / "
            }
            if(opt == "cm"){
                this.prix+= 600;
                this.commande += "Community management / "
            }
        }
    },
    components: {
        devis
    }
}
</script>