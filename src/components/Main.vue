<template>
  <main>
    <slot />
  </main>
</template>

<style scoped>
main {
  display: flex;
  flex-direction: column;
  gap: 64px;
  max-width: 1080px;
  margin: 0 auto;
}

@media (min-width: 768px) {
  main {
    gap: 200px;
  }
}

@media (min-width: 1024px) {
  main {
    gap: 320px;
  }
}
</style>
