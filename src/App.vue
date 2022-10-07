<template>
  

  
  <div id="app">
    <div>
      <nav>
        <router-link v-b-toggle.sidebar-no-header to="" >Menú</router-link>
      </nav>
      
    <b-sidebar  id="sidebar-no-header" aria-labelledby="sidebar-no-header-title" no-header shadow >
      <template #default="{ hide }" >
        <div class="p-3"  >
          <h4 id="sidebar-no-header-title"><router-link to="/">Inicio</router-link></h4>
          <p>
            Hefzi Ba Murillo Martha
            
            ITM101
            Universidad Tecnológica de Paquimé
          </p>
          <nav class="mb-3" style="font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif">
            <b-nav vertical>
              
              <b-nav-item to="/paisajes" @click="hide">Paisajes</b-nav-item>
              <b-nav-item to="/colores" @click="hide">Colores</b-nav-item>
            </b-nav>
          </nav>
          <b-button variant="dark" block @click="hide">Cerrar</b-button>
        </div>
      </template>
    </b-sidebar>
  </div>
  
    <router-view/>
  </div>

  
</template>

 
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #6e0e49;;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #6e0e49;
}

nav a.router-link-exact-active {
  color: #6e0e49;
}
.hide{
  color: #6e0e49;
}
</style>
