<template>
<div class="container">
  <div class="row">
    <div class="col-sm-6">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Création de site</h5>
          <p class="card-text">Création de site web sur mesure.</p>
          <button  class="btn btn-primary" @click="$emit('choix','creasite')">Ajouter</button>
        </div>
      </div>
    </div>
    <div class="col-sm-6">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Infographie</h5>
          <p class="card-text">Création graphique (Branding, publicités,..).</p>
          <button  class="btn btn-primary" @click="$emit('choix','graphisme')">Ajouter</button>
        </div>
      </div>
    </div>

    <div class="col-sm-6">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Montage vidéo</h5>
          <p class="card-text">Vidéo à destination de YouTube, publicités, court-métrage,...</p>
          <button  class="btn btn-primary" @click="$emit('choix','montagevideo')">Ajouter</button>
        </div>
      </div>
    </div>

    <div class="col-sm-6">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Community Management</h5>
          <p class="card-text">Gestion des réseaux sociaux, mise en place de campagnes publicitaires.</p>
          <button  class="btn btn-primary" @click="$emit('choix','cm')">Ajouter</button>
        </div>
      </div>
    </div>
    
  </div>
  
  <br>
  <div class="card">
    <p> <strong> Prix : </strong> {{total}} €</p> 
    <p> <strong> Détail de la commande :  </strong> {{detail}} </p>

    <button @click="log()" class="btn btn-primary">log console </button>
  </div>
</div>
</template>

<script>
export default {
    name : "devis",
    props:["total","detail"],

    methods :{
        log(){
            console.log(this.total);
        }
    }

}
</script>