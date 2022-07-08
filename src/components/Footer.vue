<script lang="ts" setup>
import { ref, onMounted } from 'vue'
const element = ref(null)

onMounted(() => {
  element.value.focus()
})
</script>



<template>
  <footer ref="element">
    <slot />
  </footer>
</template>

<style scoped>
footer {
  --gradient-height: 120px;
  --padding: 80px;

  --blue: #0E00FF;

  padding-inline: 40px;
  padding-top: calc(var(--gradient-height) + var(--padding));
  padding-bottom: var(--padding);
  font-family: 'IBM Plex Mono', monospace;
}
</style>
