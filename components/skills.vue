<template>
<div>
<h4>  {{nom}} </h4>
    <div>
        <div></div>
        <p> {{description}}</p>
    </div>
</div>



    
</template>

<script>
export default{
    name : 'skills',
    props : ["nom","description"]
}

</script>

<style>
.nom{
    font-size:25px;
}
.titreskill{
    font-size:25px;
}
</style>
