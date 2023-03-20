
<template>
  <header>
    <header-component/>
  </header>
    <main>
      
      <div id="titulazo">
        <h1>Promocion 2022/2023</h1>
        <h2>Desarrollo de aplicaciones web</h2>
        <h3>DAW</h3>
      </div>
      <h1>PROFESORES</h1>
      <div class="d-flex justify-content-center">
          <div v-for="item in profesores" :key="item.id">
              <fichaProfesor :profesor="item"/>
          </div>
      </div>
     <div id="alumnos2">
      <h1>Alumnos</h1>
      <div class="d-flex justify-content-center" id="alumnos">
       
          <div v-for="item in alumnos" :key="item.id">
              <fichaAlumno :alumno="item"/>
          </div>
      </div>
     </div>
      
    </main>
    <footer>
      <footer-component/>
    </footer>
    

</template>

<script>
   import headerComponent from './components/header.vue'
   import footerComponent from './components/footer.vue'
   import fichaAlumno from './components/fichaAlumno.vue'
   import fichaProfesor from './components/fichaProfesor.vue'
   import detalles from './components/DetalleAlumno.vue'

  export default{
    name: 'app',
    components: {
      headerComponent,
      footerComponent,
      fichaProfesor,
      fichaAlumno,
      detalles
    },
    data(){
      return{
        profesores: [
          {
            id:1,
            nombre: 'Juan Montero',
            foto: 'juan_montero.jpg',
            asignatura: 'Programacion',
          },
          {
            id:2,
            nombre: 'Carlos Arrebola',
            foto: 'carlos_arrebola.png',
            asignatura: 'Programacion',
          },
          {
            id:3,
            nombre: 'Ana Rovira',
            foto: 'anna_rovira.jpg',
            asignatura: 'Programacion',
          },
          {
            id:4,
            nombre: 'Jordi Egea',
            foto: 'jordi_egea.png',
            asignatura: 'Programacion',
          },
          {
            id:5,
            nombre: 'Raul Sanchez',
            foto: 'raul_sanchez.jpg',
            asignatura: 'Programacion',
          },
        ],
        alumnos: [
          {
            id: 6,
            nombre: 'Sergio Pereira',
            foto: 'Sergio.jpg',
            ciudad: 'Santa Coloma de Gramenet',
            estudios:['Grado Medio De Sistemas MicroInformaticos Y Redes'],
            trabajo:['DJ, Tecnico Informatico en Revolution Computer', 'Tecnico IT Alcampo']
          },
          {
            id: 7,
            nombre: 'Pau Diaz',
            foto: 'PauDiaz.jpg',
            ciudad: 'Badalona',
            estudios:['Grado Medio de sistemas MicroInformaticos Y Redes'],
            trabajo:['Desempleado']
          },
          {
            id: 8,
            nombre: 'Nicolas Barrio',
            foto: 'Nicolas.jpg',
            ciudad: 'Badalona',
            estudios:['Grado Medio De Sistemas MicroInformaticos Y Redes'],
            trabajo:['Tecnico Informatico ']
          },
          {
            id: 9,
            nombre: 'Jose Luis Viri Murillo',
            foto: 'horseluis.jpg',
            ciudad: 'Badalona',
            estudios:['Grado Medio De Sistemas MicroInformaticos Y Redes'],
            trabajo: ['Barrendero']
          },
          {
            id: 10,
            nombre: 'Alex Perez',
            foto: 'alexPerez.jpg',
            ciudad: 'Santa Coloma de Gramenet',
            estudios: ['Bachillerato', 'Sistemas MicroInformaticos Y Redes'],
            trabajo: ['Camarero']

          }
        ]
      }
    }
  }
</script>
  
<style>

</style>