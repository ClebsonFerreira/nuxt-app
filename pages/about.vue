<template>
 <section class="hero is-info is-fullheight">
  <div class="hero-body">
    <div class="container">
      <h1 class="title">
       Sobre
      </h1>
      <h2 class="subtitle">
       Lorem ipsum dolor, sit amet consectetur adipisicing elit. Alias quis accusantium aut sequi aliquam! Doloremque commodi quidem ipsam deserunt odit numquam mollitia ipsa animi dignissimos veritatis, illum inventore nemo dolor?
      </h2>
      <h2 class="subtitle">
       Lorem ipsum dolor, sit amet consectetur adipisicing elit. Alias quis accusantium aut sequi aliquam! Doloremque commodi quidem ipsam deserunt odit numquam mollitia ipsa animi dignissimos veritatis, illum inventore nemo dolor?
      </h2>
      <h2 class="subtitle">
       Participantes
      </h2>
      <ul>
        <li v-for="list of user" :key="list.id">
          {{list.name}}
          <ul>
            <li> Email : {{list.email}}</li>
            <li> Telefone : {{list.phone}}</li>
          </ul>
          <br>
        </li>
      </ul>
    </div>
  </div>
</section>
</template>

<script>
  export default {
    name:'about',
    data: () => {
    return {
      user:{}
    }
  },
    methods:{
    },
    async mounted () {
      const user  = await this.$axios.$get('https://jsonplaceholder.typicode.com/users');
      this.user = user;
    }
  }
</script>

<style lang="scss" scoped>

</style>
