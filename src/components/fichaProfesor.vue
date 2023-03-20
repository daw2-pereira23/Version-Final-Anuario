<template>
    <div class="card" style="width: 15rem;">
        <img :src= '"/public/imagenes/"+ profesor.foto' class="card-img-top" alt="...">
        <div class="card-body">
            <h5 class="card-title">{{profesor.nombre}}</h5>
            <p class="card-text">{{profesor.asignatura}}</p>
         
        </div>
    </div>
</template>

<script>
    export default{
        name: 'fichaProfesor',
        props:{
            profesor: Object
        }
    }
</script>

<style>

</style>