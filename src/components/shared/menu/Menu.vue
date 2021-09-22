<template>
  <nav>
    <ul>
      <li v-for="rota in rotas" v-bind:key="rota">
        <router-link :to="rota.path">
          {{ rota.titulo }}
        </router-link>
      </li>
    </ul>
  </nav>
</template>

<script>

export default {
  props: {
    rotas: {
      type: Array,
      required: true
    }
  }
};

</script>

<style>

</style>
