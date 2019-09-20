<template>
  <div class="d-none d-md-flex">
    <v-container class="proyecto1" > 
      <h1 class="proyectosTitle" >
        Proyectos
      </h1>
      <v-divider color="blue" class="divider" ></v-divider>
      <PmProyecto1/>
      <PmProyecto2/>
      <PmProyecto3/>
    </v-container>
  </div>
</template>

<script>
    import PmProyecto1 from '@/components/lista-proyectos/Proyecto1.vue'
    import PmProyecto2 from '@/components/lista-proyectos/Proyecto2.vue'
    import PmProyecto3 from '@/components/lista-proyectos/Proyecto3.vue'

  export default {
    components:{
      PmProyecto1,
      PmProyecto2,
      PmProyecto3,
    }
  }

</script>

<style lang="scss" >
.techStack1{
    background-color: black;
}

h1{
  font-size: 40px;
    margin-top: 10px;
    margin-bottom: 0px;
    color: rgb(0, 0, 0);
}

h2{
    color: #ffff;
}
.titleList{
    color: rgb(47, 0, 255);
}
.subtitle{
    color:white;
}
.title2{
    color: rgb(47, 0, 255) 
}
.divider{
  margin-top:15px;
  margin-bottom: 15px;
.proyectosTitle{
    margin-bottom: -15px;
  }

.btnLeft{
    margin-right: 20px;
  }
.btnRight{
    margin-left: 2em;
  }
}


</style>

// componente de cada proyecto 
Esta aplicación es una plataforma de Esports en la cual puedes crear tus torneos con fecha y hora.
cuando creas tú torneo automaticamente se agrega a la lista de torneos y otros usuarios se pueden registrar.

