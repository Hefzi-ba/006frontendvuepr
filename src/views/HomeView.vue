<template>
  <div class="home">
    <CardInd/>
    <TablasN/>
    
    <b-card bg-variant="dark" text-variant="white" title="Footer">
  <b-card-text>
    Esto deberia ser un footer
  </b-card-text>
  <b-button href="#" variant="primary">Reservamos Politicas </b-button>
</b-card>
    
    
  </div>
 
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import CardInd from '../components/CardInd.vue'

import TablasN from '@/components/TablasN.vue'


export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    CardInd,
    TablasN
}
}
</script>
