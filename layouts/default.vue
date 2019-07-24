<template>
  <div>
    <Menu />
    <nuxt />
    <section class="hero is-dark">
      <div class="hero-body">
        <div class="container">
          <div class="columns">
            <div class="column">
              <h2 class="title">Contatos</h2>
              <ul>
                <li class="subtitle">teste</li>
                <li class="subtitle">teste</li>
                <li class="subtitle">teste</li>
              </ul>
            </div>
            <div class="column">
               <h2 class="title">Redes sociais</h2>
              <ul>
                <li class="subtitle">teste</li>
                <li class="subtitle">teste</li>
                <li class="subtitle">teste</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import Menu from "~/components/Menu.vue";
export default {
  components: {
    Menu
  }
};
</script>
