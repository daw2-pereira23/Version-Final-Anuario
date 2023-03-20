<template>
    <div class="card" style="width: 15rem;">
        <router-link :to="{name:'detalles/:id', params:{id:alumno.id}}"><img :src='"/public/imagenes/"+alumno.foto' class="card-img-top img-fluid"></router-link>
        <div class="card-body">
            <h5 class="card-title">{{alumno.nombre}}</h5>
            <p class="card-text">{{alumno.ciudad}}</p>
            <a href="#" class="btn btn-primary" id="saberMas">Saber mas</a>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'fichaAlumno',
        props:{
            alumno: Object
        }
    }

    
    

</script>

<style>

</style>