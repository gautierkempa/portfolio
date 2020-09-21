<template>
  <!-- test code louis -->

  <div>
    <div class="card-deck zoom">
        <div class="card">   
            <img :src="src2" class="card-img-top">    
                <div class="card-body">
                    <h5 class="card-title"> {{ h12 }} </h5>  
                    <p class="card-text"> {{ text2 }} </p>
                    <p style="margin-left:18%" class="card-text"></p>
                    
                </div>
        </div>
        
    </div>
    
    
    
 </div>
</template>

<script>
export default{
    name : 'realisation',
    props : ["src2", "text1", "h12", "href2", "mavideo2"]
}

</script>
<style scoped>

.zoom {
 
  
  transition: transform .3s; /* Animation */

  margin: 0 auto;
}

.zoom:hover {
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}
.card{
    margin-bottom:15px;
}
</style>

