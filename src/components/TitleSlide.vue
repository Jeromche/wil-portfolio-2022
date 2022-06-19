<script setup lang="ts">
interface Props {
  line: string;
}

defineProps<Props>()
</script>

<template>
  <span class="outer">
    <span class="inner">
      {{ line }}
    </span>
  </span>
</template>

<style scoped>
@keyframes slide-up {
  0% {
    transform: translateY(100%);
  }

  25% {
    transform: translateY(100%);
  }

  100% {
    transform: translateY(0);
  }
}

.outer {
  display: block;
  overflow: hidden;
  height: 1.3em;
}

.inner {
  display: block;
  animation: slide-up 1s cubic-bezier(0, 0.8, 0.2, 1);
}
</style>
