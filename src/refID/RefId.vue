<script setup lang="ts">
import {ref} from 'vue';
import type { Ref } from 'vue';
const input: Ref<HTMLInputElement> = ref(null)

const handleClick = ():void => {
  const disabled = input.value.disabled
  input.value.disabled = !disabled;
}

</script>

<template>
<input ref="input" ></input>
<button @click='handleClick' >activar/desactivar</button>
</template>

<style scoped></style>
