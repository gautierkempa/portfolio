<template>
<div>
<title> CV | Gautier Kempa</title>
<meta name="description" content="Monteur vidéo freelance YouTube, publicités,etc." />
  <!-- Page Container -->
  <div class="w3-content w3-margin-top down" style="max-width:1400px;">

    <!-- The Grid -->
    <div class="w3-row-padding">

      <!-- Left Column -->
      <div class="w3-third">

        <div class="w3-white w3-text-grey w3-card-4">
          <div class="w3-display-container">
            <img src="../image/gautier2.jpg" style="width:70%" alt="Avatar">

          </div>
          <div class="w3-container">
            <h2>Kempa Gautier</h2>
            <p><i class="fa fa-briefcase fa-fw w3-margin-right w3-large w3-text-teal"></i>Etudiant et freelance</p>
            <p><i class="fa fa-home fa-fw w3-margin-right w3-large w3-text-teal"></i>Belgique, Dour</p>
            <p><i class="fa fa-envelope fa-fw w3-margin-right w3-large w3-text-teal"></i>gautierkempapro@gmail.com</p>
            <hr>

            <p class="w3-large"><b><i class="fa fa-asterisk fa-fw w3-margin-right w3-text-teal"></i>Compétences</b></p>
      
            
            <skills v-for="skill in skills" :nom="skill.nom" :description="skill.description" />
            <br>

            <p class="w3-large w3-text-theme"><b><i
                  class="fa fa-globe fa-fw w3-margin-right w3-text-teal"></i>Langues</b></p>
            <p>Français</p>
            <div class="w3-light-grey w3-round-xlarge">
              <div class="w3-round-xlarge w3-teal" style="height:24px;width:100%"></div>
            </div>
            <p>Anglais</p>
            <div class="w3-light-grey w3-round-xlarge">
              <div class="w3-round-xlarge w3-teal" style="height:24px;width:90%"></div>
            </div>
            <p>Espagnol</p>
            <div class="w3-light-grey w3-round-xlarge">
              <div class="w3-round-xlarge w3-teal" style="height:24px;width:60%"></div>
            </div>
            <p>Néerlandais</p>
            <div class="w3-light-grey w3-round-xlarge">
              <div class="w3-round-xlarge w3-teal" style="height:24px;width:40%"></div>
            </div>
            <br>
          </div>
        </div><br>

        <!-- End Left Column -->
      </div>

      <!-- Right Column -->
      <div class="w3-twothird">


        <div class="w3-container w3-card w3-white w3-margin-bottom">
          <experience v-for="exp in exps" :date="exp.date" :titre="exp.titre" :desc="exp.desc" />
        </div>

        <div class="w3-container w3-card w3-white">
          <h2 class="w3-text-grey w3-padding-16"><i
              class="fa fa-certificate fa-fw w3-margin-right w3-xxlarge w3-text-teal"></i>Parcours Scolaire</h2>
          <div class="w3-container">
            <h5 class="w3-opacity"><b>E-business // Heph Condorcet Froyennes</b></h5>
            <h6 class="w3-text-teal"><i class="fa fa-calendar fa-fw w3-margin-right"></i> <span
                class="w3-tag w3-teal w3-round">Actuellement</span> </h6>
            </h6>
            <p>Etudes dédiées au monde du web et portées vers l'avenir.</p>
            <hr>
          </div>
          <div class="w3-container">
            <h5 class="w3-opacity"><b>Institut la Sainte-Union (Dour)</b></h5>
            <h6 class="w3-text-teal"><i class="fa fa-calendar fa-fw w3-margin-right"></i>2012- 2018</h6>
            <p>Obtention du CESS</p>
            <hr>
          </div>

        </div>

        <!-- End Right Column -->
      </div>

      <!-- End Grid -->
    </div>
    

    <!-- End Page Container -->
  </div>
</div>
</template>

<script>
import experience from '@/components/experience.vue'
import skills from '@/components/skills.vue'

export default{
  components : {
    experience,skills
  },

data (){
  return {
    // expériences // 
    exps : [{
      date : "Mai 2018 - Actuellement",
      titre : "Gestionnaire chaine YouTube / Monteur vidéo pour LRB - Solary",
      desc : " Gestion de la chaine YouTube, de la communication et du montage vidéo."
    },
    {
       date : "Juillet 2017 - Actuellement",
      titre : "Monteur vidéo freelance",
      desc : " Clients : Domingo, LRB, Zack Nani, OkaMedia, Ruurk, SoThomas, Sparkdise, Kotei&Kameto, Morgan Charriere,..."
    }
   ],
    
    // compétences
    skills: [{
          nom: ' Montage vidéo ',
          description : 'Montages et travail de post-production ',
        },
        {
          nom: ' Graphisme ',
          description : 'Créations graphiques ',
        },
        {
          nom: ' Développement ',
          description : 'Création de sites web / front-end'
        },
        {
          nom: ' Community Manager ',
          description : 'Gestion de réseaux sociaux'
        },
        {
          nom: ' Motion design ',
          description : 'Animations '
        },
      ]
    }
  }
}
</script>

<style>
.down { 
    padding-top: 65px; 
}
</style>