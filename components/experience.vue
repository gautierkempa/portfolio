<template>   
<div class="w3-content w3-margin-top" style="max-width:1400px;">
    <div >
            <!-- ça fonctionne après ça -->
      <div class="">
      <h2 class="w3-text-grey ">Expérience</h2>
            <div class="w3-container">
                <h5 class="w3-opacity"><b>{{titre}}</b></h5>
                <h6 class="w3-text-teal"><i class="fa fa-calendar fa-fw w3-margin-right"></i>{{date}}</h6>
                <p>{{desc}} </p>
                <hr>
            </div>
    <!-- ça fonctionne avant -->
         </div>
      </div>
    </div>

</div>
</template>

<script>
export default{
    name : 'experience',
    props : ["date", "desc", "titre"]
}

</script>

<style>

</style>
