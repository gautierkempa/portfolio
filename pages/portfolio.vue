<template>
<div class="container down">
<title> Portfolio | Gautier Kempa</title>
<meta name="description" content="Monteur vidéo freelance YouTube, publicités,etc." />
<h1 class="text-center text-monospace reveal-text">Mes réalisations </h1>
<p class="text-center">Présentation des différentes prestations que j'ai pu réaliser </p>
      <div class="card-deck">
            <realisation style="margin-left:auto; width:auto;" v-for="img in imgs" :h1="img.h1" :text="img.text" :src="img.src" :href="img.href" :mavideo="img.mavideo" />
      </div>
</div>
</template>

<script>
 import realisation from '@/components/realisation.vue'
 

  export default {
    components: {
      realisation, 
    },


    data() {
      // réalisations // 
      return {
        imgs: [{
            text : "Vidéo pour Domingo",
            h1 : "Montage Vidéo",
            mavideo : "https://www.youtube.com/embed/INpFj05fY2E"

          },

          {
           text : "Vidéo pour LRB ",
            h1 : "Montage Vidéo",
            mavideo : "https://www.youtube.com/embed/yYIh3rD3xl0"
          },
          {
            text : "Vidéo pour Kameto ",
            h1 : "Montage Vidéo",
            mavideo : "https://www.youtube.com/embed/Ssd935QUF00"
            

          },
          {
            text : "Vidéo pour Morgan Charriere ",
            h1 : "Montage Vidéo",
            mavideo : "https://www.youtube.com/embed/xp5mGrCvI1w"
            

          },
          {
            text : "Vidéo pour Ruurk ",
            h1 : "Montage Vidéo",
            mavideo : "https://www.youtube.com/embed/G7Yb-CIIlFk"
            

          },
          {
            text : "Vidéo pour SoThomas",
            h1 : "Montage Vidéo",
            mavideo : "https://www.youtube.com/embed/yvx0sZ35NyE"

          },
          {
            text : "Vidéo pour Sparkdise",
            h1 : "Montage Vidéo",
            mavideo: "https://www.youtube.com/embed/rBWy9O-47B8"

          },
          {
            
            text : "Vidéo pour Zack Nani",
            h1 : "Montage Vidéo",
            mavideo : "https://www.youtube.com/embed/yMRepyjiRXs"

          },
          {
            
            text : "Promotion de PassionZ",
            h1 : "Montage Vidéo",
            mavideo : "https://www.facebook.com/plugins/video.php?href=https%3A%2F%2Fwww.facebook.com%2FPassionzEntrepreneurs%2Fvideos%2F2068121213513450%2F&show_text=0&width=560" 

          },
          {
            
            text : "Voir la playlist complète ainsi que la vidéo plus récente",
            h1 : "Montage Vidéo",
            mavideo : "https://www.youtube.com/embed/videoseries?list=PLKLe3OKFQ3JaAX6dkOU82wZw98tl1nhJY"

          }           

        ],
      }
    }



  }

</script>

<style scoped>
.card-deck{
    
}


/* animation texte titre */
:root {
	--delay: 0;
	--duration: 800ms;
	--iterations: 1;
}
/* •·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•·•· */


.reveal-text,
.reveal-text::after {
	animation-delay: var(--animation-delay, 2s);
	animation-iteration-count: var(--iterations, 1);
	animation-duration: var(--duration,2000ms);
	animation-fill-mode: both;
	animation-timing-function: cubic-bezier(0.0, 0.0, 0.2, 1);
}

.reveal-text {
	--animation-delay: var(--delay, 0);
	--animation-duration: var(--duration, 2000ms);
	--animation-iterations: var(--iterations, 1);
	position: relative;
	font-size: 30px;
	animation-name: clip-text;
	color: black;
	white-space: nowrap;
	cursor: default;
	
	&::after {
		content: "";
		position: absolute;
		z-index: 999;
		top: 0;
		left: 0;
		right: 0;
		bottom: 0;
		background-color: #f2f98b;
		transform: scaleX(0);
		transform-origin: 0 50%;
		pointer-events: none;
		animation-name: text-revealer;
	}
	
}


@keyframes clip-text {
	from {
		clip-path: inset(0 100% 0 0);
	}
	to {
		clip-path: inset(0 0 0 0);
	}
}


@keyframes text-revealer {
	
	0%, 50% {
		transform-origin: 0 50%;
	}
	
	60%, 100% {
		transform-origin: 100% 50%;		
	}

	
	60% {
		transform: scaleX(1);
	}
	
	100% {
		transform: scaleX(0);
	}
}

.down { 
    padding-top: 65px; 
}
/* animation texte reveal */












</style>
