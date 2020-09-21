<template>
    <div class="down">
    <title> Contact | Gautier Kempa</title>
    <meta name="description" content="Monteur vidéo freelance YouTube, publicités,etc." />
    <h4 class="text_form">Si vous souhaitez me contacter, veuillez remplir le formulaire ci-dessous</h4>
           <form id="contactForm" onsubmit="return validate()" action="contact.php" method="post">
              
              <input class="formInput" type="text" id="name" name="name" autocorrect="off" placeholder="Nom"/>
              <input class="formInput" type="email" name="email" id="email" autocapitalize="off" autocorrect="off" placeholder="E-mail"/>
              <textarea class="formInput" name="message" id="message" placeholder="Message" ></textarea>
             
              <br>
              <input class="submitForm" type="reset" value="Supprimer votre message" />
              <input class="submitForm" type="submit" value="Envoyer"/>
           
           </form>

    </div>
</template>

<script>

</script>

<style>

.text_form{
    text-align:center;
    color:black;
}



  #contactForm {
      margin: 0 auto;
}

  #contactForm input, textarea {
      letter-spacing: 2px;
      font: 200 1em/1.1em 'Helvetica Neue', sans-serif;
      
      color: #000;
      background-color: RGBA(204, 204, 204, .1);
    
      outline: none; border: none;
   
      display:block;
      margin: 0 auto;
      padding: 1em;
      width: 90%;
      max-width: 400px;
 }

#contactForm textarea {
  height: 150px;
}

#contactForm *:focus {
   background-color: #dfe6e9;
}

#contactForm *:hover {
   background-color: #dfe6e9;
}

::-webkit-input-placeholder {
      color: #777;
}

:-moz-placeholder { /* Firefox 18- */
      color: #777; 
}

::-moz-placeholder {  /* Firefox 19+ */
    color: #777; 
}

:-ms-input-placeholder {  
       color: #777;
}

.down { 
    margin-top: 14px; 
}
</style>