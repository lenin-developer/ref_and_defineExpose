<script setup lang="ts">
import { type Ref, ref } from 'vue';
import type ChildrenComponent from './ChildrenComponent.vue';
const refComponentChil: Ref<InstanceType<typeof refComponentChil>> = ref(null);

const recalcular = () => {
  refComponentChil.value.recalculatePorcentage();
};
</script>

<template>
  <ChildrenComponent ref="refComponentChil" />
  <button @click="recalcular">Terminar</button>
</template>

<style scoped></style>
