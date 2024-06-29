<script setup lang="ts">
import VueIcon from './components/VueIcon.vue'
import ControlDelegadoPorReferencia from './controlDelegadoPorReferencia/ControlDelegadoPorReferencia.vue';
import RefId from './refID/RefId.vue'


</script>

<template>
  <div>
    <VueIcon />
    <h2>ref (id)</h2>
    <RefId/>
    <hr>
    <h2>control delegado por referencia</h2>
    <ControlDelegadoPorReferencia />

  </hr>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
