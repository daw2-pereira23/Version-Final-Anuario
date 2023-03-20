<template>
      <header>
        <nav class="navbar navbar-expand-lg bg-body-tertiary col-12">
          <div class="col-2 d-flex justify-content-start">
           <img src="/imagenes/logo_fpllefia.png" alt="Logo fp llefia" id="logotipo">
          </div>
          <div class="col-10 text-end">
            <p>Sergio Pereira Hidalgo</p>
          </div>
        </nav>
      </header>
</template>

<script>
  export default {
    name: 'header-component',
  }
</script>

<style>
    #logotipo{
      width: 175px;
    }
</style>