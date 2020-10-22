<template>
  <div>
    <h2>{{ currentValue }}</h2>
    <button @click="increment">+</button>
    <button @click="decrement">-</button>
  </div>
</template>

<script>
  export default {
    methods: {
      increment() {
        this.$store.commit('INCREMENT_COUNTER');// on utilise la variable $store pour la mutation, commiter une action pour modifier le state.
      },
      decrement() {
        this.$store.commit('DECREMENT_COUNTER');
      }
    },
    computed: {
      currentValue() {
        return this.$store.state.currentValue;
      }
    },
  }
</script>

<style scoped>

</style>