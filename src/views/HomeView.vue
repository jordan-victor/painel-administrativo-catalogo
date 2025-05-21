<template>
  <main>
  <header>
    <LinksView/>
  </header>

    <router-link :to="{name:'cadastro'}">
      <div class="card">
        CADASTRO SEU ESTABELECIMENTO
      </div>
    </router-link>
  </main>
</template>

<script>
// @ is an alias to /src
import LinksView from '../components/LinksView.vue'

export default {
  name: 'HomeView',
  components: {
    LinksView
  }
}
</script>
