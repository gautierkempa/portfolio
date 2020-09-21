<template>
  <!-- test code louis -->

  <div class="container-fluid">
  <center>
   <div class="card-deck zoom float-none">
        <div class="card" style="width: 18rem;">   
            <div class="embed-responsive embed-responsive-16by9">
                 <iframe class="card-img-top embed-responsive-item embed-responsive embed-responsive-16by9" width="649" height="364" v-bind:src="mavideo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>                
                <div class="card-body">
                    <h5 class="card-title"> {{ h1 }} </h5>  
                    <p class="card-text"> {{ text }} </p>
                    <p class="card-text"></p>
                </div>
        </div>
    </div>
    <img :src="src" class="card-img-top">
  </center>
   
</div>
</template>

<script>
export default{
    name : 'realisation',
    props : ["src", "text", "h1", "href", "mavideo"]
}

</script>
<style scoped>

.zoom {
 
  
  transition: transform .3s; /* Animation */

  margin: 0 auto;
}

.zoom:hover {
  transform: scale(1.1);
}
.card{
    
}
</style>

