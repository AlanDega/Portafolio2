<template>
<div >
  <v-container fluid class="hero" align-items="center" fill-height >
    <v-row justify="center" align="center" class="row1">
      <v-col cols="9" justify="center" align="center">
        <IntroMobile/>
        <Intro/>
      </v-col> 
    </v-row>
  </v-container>
  <div class="caru">
 <CertCarousel/>

  </div>

  </v-container>
  <!-- <CertGrid/> -->
  <v-container>
    <v-row align="center" justify="center" >
      <v-btn dark href="https://platzi.com/@alandega/">Ver todos los certificados</v-btn>
      <!-- on hover goes to purple -->
    </v-row>
  </v-container>
  <Proyectos/>
  <ProyectosMobile/>
  <v-row align="center" justify="center">
    <v-btn dark class="btnProyectos" href="https://github.com/AlanDega">Ver todos los proyectos</v-btn>
  </v-row>
  <div class="d-none d-md-flex">
    <Footer/>
  </div>
  <div class="d-flex d-sm-flex d-md-none">
    <FooterMobile/>
  </div>
</div>
</template>



<script>
import CertGrid from '@/components/CertGrid.vue'
import CertCarousel from '@/components/CertCarousel.vue'
import Footer from '@/components/layout/Footer.vue'
import FooterMobile from '@/components/layout/FooterMobile.vue'
import ProyectosMobile from '@/components/ProyectosMobile.vue'
import Proyectos from '@/components/Proyectos.vue'
import Intro from '@/components/Intro.vue'
import IntroMobile from '@/components/IntroMobile.vue'


  export default {
    components:{
      Intro,
      IntroMobile,
      CertGrid,
      CertCarousel,
      Proyectos,
      ProyectosMobile,
      Footer,
      FooterMobile
    },
    data: () => ({
      
    }),

  }     
      
</script>
<style>
.caru{
}
.hero{
  background-color: #060715;
  width: 100%;
    font-size: 30px;

  
}

.whiteText{
  color: #FFFF;
}
.purpleText{
  color: #4200FF;
  
}
.greenText{
  color: #00FFA3;
}
.blueText{
  color: #00C2FF;
}

.proPic{
  height: 90px;
  width: 90px;
  border-radius: 50%;
  margin-bottom: 20px;
}
.btnProyectos 
{
  margin-top: 10px;
  margin-bottom: 30px;
}




</style>

if mobile only one card component and hide grid component 
