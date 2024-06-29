<script setup lang="ts">
import { ref, defineExpose } from 'vue';
import type { Ref } from 'vue';
const porcentaje: Ref<number> = ref(0);

const recalculatePorcentage = (): void => {
  porcentaje.value = 100;
};

//expone una funcion,componente,propiedad, etc para poder acceder externamente
defineExpose({ recalculatePorcentage });
</script>

<template>
  <h4>porcentaje {{ porcentaje }}%</h4>
</template>

<style scoped></style>
