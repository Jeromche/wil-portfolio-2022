<template>
  <div class="animation" />
</template>

<style scoped>
@keyframes rotate {
  0% {
    transform: rotate(0deg);
  }

  100% {
    transform: rotate(360deg);
  }
}

.animation {
  --size: 700px;

  position: fixed;
  top: 200px;
  left: 50%;
  transform: translateX(600px);
  width: var(--size);
  height: var(--size);
  filter: blur(calc(var(--size) / 5));
  background-image: linear-gradient(#37eba9d9, #5b37eb);
  animation: rotate 50s cubic-bezier(0.8, 0.2, 0.2, 0.8) alternate infinite;
  border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
  z-index: -1;
}
</style>
