<template>
  <div>
  <title> Accueil | Gautier Kempa</title>
  <meta name="description" content="Monteur vidéo freelance YouTube, publicités,etc." />
  <!-- test  -->
  <header class="masthead">
            <div class="container h-100">
                <div class="row h-100 align-items-center justify-content-center text-center">
                    <div class="col-lg-10 align-self-end">
                        <h1 class="text-uppercase text-white font-weight-bold">Gautier Kempa</h1>
                        <hr class="divider my-4" />
                    </div>
                    <div class="col-lg-8 align-self-baseline">
                        <h2 class="text-white font-weight-bold mb-5"> Bonjour ! Je m'appelle Gautier Kempa, je suis freelance et étudiant en e-Business.</h2>
                        <a class="btn  btn-danger btn-xl js-scroll-trigger" href="#drop">En savoir plus </a>
                    </div>
                </div>
            </div>
        </header>
        <!-- About-->
       
   
  <!-- test -->  

    <!-- image + texte présentation -->
   
     
<!-- test --> 
<br> <br>
 <div class="zoom">
    <div class="container bg-dark" id="drop">
        <div class="row">
            <div class="col-xl-12">
                <div class=" text-center">
                    <h2 class="animated bounce text-white" >Je suis un freelance créatif basé en belgique.</h2>
                </div>
            </div>
        </div>
        <div class="row">
            <div class="col-lg-12 col-md-12 text-center">
                
                    <p class="textepresentation" >Depuis mon plus jeune âge, le monde de la création, de la vidéo et d'internet me passionne. 
                    </p>
                    <p class="textepresentation">Pratiquant le montage vidéo depuis mes 13 ans, c'est en 2018 que j'ai décidé de me lancer en tant que freelance et d'entamer des études en e-business </p>
            </div>
        </div> 
    </div>
 </div>
<br>
<!-- -->
<center>
<div class="container realisationss">
<h3 class="text-center reveal-text ">Aperçu de mes réalisations </h3>
      <div class="card-deck ">
            <realisation style="margin-left:50px; width:25%;" v-for="img in imgs" :h1="img.h1" :text="img.text" :src="img.src" :href="img.href" :mavideo="img.mavideo" />
      </div>
      <a class="btn btn-secondary" href="portfolio" role="button">En voir plus</a>
      <br>
</div>
</center>

<!-- --> 

<div class="container">
<div class="row">
    <div class="col-md-6 "> 
      <div class="text-center reveal-text">
        <div class=" w3-text-black ">
          <div>
              <h3 ><b>Compétences</b></h3>          
              <skills v-for="skill in skills" :nom="skill.nom" :description="skill.description" />
              <a class="btn btn-secondary" href="cv" role="button">En savoir plus</a>
          </div>
        </div>
      </div>
    </div>

    <div class="col-md-6">
    <br>
        <div class="card text-white bg-dark" style="max-width: 28rem;">
            <div class="card-body">
              <h5 class="card-title">freelance et étudiant</h5>
              <p class="card-text">Grâce à mon activité de freelance et mes études en e-Business, j'ai développé des compétences dans divers domaines.</p>
            </div>
      </div>
    </div>

</div>
</div>








<!-- -->
<br>


 
    <!-- -->
  <br>
     <div class="site-section bg-light">
      <div class="container">
        <div class="row justify-content-center text-center mb-5">
          <div class="col-12 text-center mb-12">
            <h2 class="text-center">Ils me font confiance ! </h2>
          </div>
        </div>


        <div class="row">
          <div class="col-lg-4 mb-4 mb-lg-0 sm-12">
            <div class="testimonial-2">
              <div class="d-flex v-card align-items-center mb-4 ">

              
                <img src="../image/domingo.jpg" alt="Image" class="img-fluid mr-3 clients clip-circle ">
              
                <a  href="https://www.youtube.com/user/ElDom1nG0"  target="_blank">
                <p class="font-weight-bolder">Domingo  <br> <img style="width:20%" src="../image/ytb2.png"> <span class="youtube">600 K </span> </p>  </a>            
              </div>
            </div>
          </div>


          <div class="col-lg-4 mb-4 mb-lg- sm-12">
            <div class="testimonial-2">
              <div class="d-flex v-card align-items-center mb-4">
                <img src="../image/lrb.jpg" alt="Image" class="img-fluid mr-3 clients clip-circle">
                <a  href="https://www.youtube.com/user/lrbetsarens"  target="_blank">
                <p class="font-weight-bolder">LRB  <br> <img style="width:20%" src="../image/ytb2.png"> <span class="youtube">280 K </span> </p> </a>
              </div>


            </div>
          </div>
          <div class="col-lg-4 mb-4 mb-lg-0 sm-12">
            <div class="testimonial-2">
              <div class="d-flex v-card align-items-center mb-4" >
                <img src="../image/thomas.jpg" alt="Image" class="img-fluid mr-3 clients clip-circle" >
                <a  href="https://www.youtube.com/channel/UCNcpg5888UgFfRVVzrLr8DQs"  target="_blank">
                <p class="font-weight-bolder">SoThomas <br> <img style="width:20%" src="../image/ytb2.png"> <span class="youtube">172 K </span> </p>  </a>
              </div>  
            </div>
          </div>
          <div class="col-lg-4 mb-4 mb-lg-0 sm-12">
            <div class="testimonial-2">
              <div class="d-flex v-card align-items-center mb-4">
                <img src="../image/ruurk.jpg" alt="Image" class="img-fluid mr-3 clients clip-circle">
                <a  href="https://www.youtube.com/channel/UCL1QMoH46aJrsfSNE2FmsYQ"  target="_blank">
                <p class="font-weight-bolder">Ruurk <br> <img style="width:20%" src="../image/ytb2.png"> <span class="youtube">30 K </span> </p>  </a>
              </div>  
            </div>
          </div>
          <div class="col-lg-4 mb-4 mb-lg-0 sm-12">
            <div class="testimonial-2">
              <div class="d-flex v-card align-items-center mb-4">
                <img src="../image/zack.jpg" alt="Image" class="img-fluid mr-3 clients clip-circle">
                  <a  href="https://www.youtube.com/channel/UCSJxne19pJyW7l7HjHM-LRg"  target="_blank">
                <p class="font-weight-bolder">Zack Nani<br> <img style="width:20%" src="../image/ytb2.png"> <span class="youtube">420 K </span> </p>  </a>
              </div>  
            </div>
          </div>
          <div class="col-lg-4 mb-4 mb-lg-0 sm-12">
            <div class="testimonial-2">
              <div class="d-flex v-card align-items-center mb-4">
                <img src="../image/morgan.jpg" alt="Image" class="img-fluid mr-3 clients clip-circle">
                <a  href="https://www.youtube.com/channel/UCBfJ3F2OJgctIyfnSL0LoRw"  target="_blank">
                <p class="font-weight-bolder">Morgan Charriere<br> <img style="width:20%" src="../image/ytb2.png"> <span class="youtube">70 K </span> </p>  </a>
              </div>  
            </div>
          </div>

        </div>
      </div>
    </div>  
    
    <div class="container">
      <div >
         <p></p>
        <h3 class="text-center">Travaillons ensemble !</h3>
        <div class="text-center">
          <a class="btn btn-secondary" href="contact" role="button">Contactez-moi</a>
          <br>
          <p></p>
        </div>
        

      </div>
    </div>
   


    

    
        <!-- End Left Column -->
     
<!-- test email -->


<!-- footer -->
<!-- Footer -->
<footer class="page-footer font-small blue pt-4">

  <!-- Footer Links -->
  <div class="container-fluid text-center text-md-left">

    <!-- Grid row -->
    <div class="row">

      <!-- Grid column -->
      <div class="col-md-2 mt-md-0 mt-1"></div>
      <div class="col-md-4 mt-md-0 mt-3">

        <!-- Content -->
        <h5 class="text-uppercase">Gautier Kempa</h5>
        <p>Site web développé avec Vue.js dans le cadre du cours de Software Developpement.</p>

      </div>
      <!-- Grid column -->

      <hr class="clearfix w-100 d-md-none pb-3">

      <!-- Grid column -->
      <div class="col-md-3 mb-md-0 mb-3">

        <!-- Links -->
        <h5 class="text-uppercase">Liens</h5>

        <ul class="list-unstyled">
          <li>
            <a href="portfolio">Portfolio</a>
          </li>
          <li>
            <a href="cv">CV</a>
          </li>
          <li>
            <a href="contact">Contact</a>
          </li>
           <li>
            <a href="https://twitter.com/GautierGT7" target="_blank">Twitter</a>
          </li>
          <li>
            <a href="https://be.linkedin.com/in/gautier-kempa-71a933162" target="_blank">LinkedIn</a>
          </li>



        </ul>

      </div>
      <div style="margin-left:-5%" class="col-md-2 mb-md-0 mb-2">
        <button  class="btn btn-xl btn-dark" @click="showtext = !showtext">Afficher mon adresse mail </button>
        <mail v-if="showtext" />
        <br>
      </div>

    </div>
  </div>
</footer>
<!-- Footer -->


  </div>
</template>

<script>
  import skills from '@/components/skills.vue';
  import realisation from '@/components/realisation.vue'
  import mail from '@/components/email.vue'

  export default {
    components: {
      skills, realisation,mail
    },


    data() {
      return {
        skills: [{
          nom: ' Montage vidéo ',
          description : 'Montage / Motion Design',
        },
        {
          nom: ' Graphisme ',
          description : 'Créations graphiques ',
        },
        {
          nom: ' Développement ',
          description : 'Création de site web / front-end'
        },
      ],

        imgs: [{
            text : "Vidéo pour Domingo",
            h1 : "Montage Vidéo",
            mavideo : "https://www.youtube.com/embed/INpFj05fY2E"

          },
            {
            text : "Vidéo pour SoThomas",
            h1 : "Montage Vidéo",
            mavideo : "https://www.youtube.com/embed/yvx0sZ35NyE"

          },
          { 
            text : "Promotion de PassionZ",
            h1 : "Montage Vidéo",
            mavideo : "https://www.facebook.com/plugins/video.php?href=https%3A%2F%2Fwww.facebook.com%2FPassionzEntrepreneurs%2Fvideos%2F2068121213513450%2F&show_text=0&width=560" 

          },
        ],
        // pour l'email // 
        showtext:false,
      }
    }



  }

  


  

</script>

<style>
html {
  scroll-behavior: smooth;
}
body {
  
}

footer{
  color: #dcdde1;
  background-color :#353b48 ;
}

.textepresentation{
  color:#f1f2f6;
}


.zoom {
 
  
  transition: transform .5s; /* Animation */

  margin: 0 auto;
}

.zoom:hover {
  transform: scale(1.1);
}

.clip-circle {
  clip-path: circle(80px at center);
}
/* test page full screen */ 
header.masthead {
  padding-top: 10rem;
  padding-bottom: calc(10rem - 4.5rem);
  background: linear-gradient(to bottom, rgba(92, 77, 66, 0.8) 0%, rgba(92, 77, 66, 0.8) 100%), url("../image/gautierpic2.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-attachment: scroll;
  background-size: cover;
}
header.masthead h1 {
  font-size: 2.25rem;
}
@media (min-width: 992px) {
  header.masthead {
    height: 100vh;
    min-height: 40rem;
    padding-top: 4.5rem;
    padding-bottom: 0;
  }
  header.masthead p {
    font-size: 1.15rem;
  }
  header.masthead h1 {
    font-size: 3rem;
  }
}
@media (min-width: 1200px) {
  header.masthead h1 {
    font-size: 3.5rem;
  }
}

    /* test navbar page full screen */
     


    /* fin test nav bar page full screen */



/* fin page full screen*/

  .bonjour {
    font-size: 33px;
   
  }
  .p{
      font-color: white;
  }

  

  .ensavoirplus {
    font-size: 40px;
  }


.clients{
    width:50%;
}

.youtube{
  color:#c0392b;
}


p {
    font-size: 20px;
}

p.small {
    font-size: 16px;
}


h1,
h2,
h3,
h4,
h5,
h6 {
    text-transform: uppercase;
    font-family: 'Ubuntu',"Helvetica Neue",Helvetica,Arial,sans-serif;
    font-weight: 700;
}

@media(max-width:767px) {
    section {
        padding: 25px 0;
    }

    section.first {
        padding-top: 75px;
    }
}

@media(min-width:767px) {
    #portfolio .col-sm-3 {
        padding-right:0;
        padding-left: 0;
    }
} 
</style>
