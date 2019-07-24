<template>
  <nav class="navbar navbar-custom" role="navigation" aria-label="main navigation">
    <div class="container">
      <div class="navbar-brand">
      <nuxt-link to="/" class="navbar-item logo">Camará<span>Tech</span></nuxt-link>
        <a role="button" @click="navOpen" class="navbar-burger burger" :class="{ 'is-active': isActive }" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>
      <div id="navbarBasicExample" class="navbar-menu " :class="{ 'is-active': isActive }">
        <div class="navbar-end">
          <nuxt-link to="/" class="navbar-item">Home</nuxt-link>
          <nuxt-link to="/about" class="navbar-item">Sobre</nuxt-link>
          <nuxt-link to="/portfolio" class="navbar-item">Portfolio</nuxt-link>
          <nuxt-link to="/contact" class="navbar-item">Contato</nuxt-link>
        </div>
      </div>
  </div>
</nav>
</template>
<script>
  export default {
    name:'Menu',
    data: function() {
      return {
        isActive: false
      }
    },
    methods:{
      navOpen:function(){
        this.isActive = !this.isActive;
      },
    }
  }
</script>
<style>
.logo{
  font-size: 20px;
  color:grey;
}
.logo span{
  color:#42b983;
}
.navbar-custom{
 color:grey;
 box-shadow: 1px 1px 5px grey;
}
.navbar-custom a:hover{
  color:#42b983;
}

</style>



