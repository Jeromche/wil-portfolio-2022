<template>
  <div class="container">
    <div class="animation" />
  </div>
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

.container {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 1200px;
  overflow: hidden;
  z-index: -1;
}

.animation {
  --size: 600px;

  position: absolute;
  top: 200px;
  left: 50%;
  transform: translateX(600px);
  width: var(--size);
  height: var(--size);
  filter: blur(calc(var(--size) / 5));
  background-image: linear-gradient(#37eba9d9, #5b37eb);
  animation: rotate 80s cubic-bezier(0.8, 0.2, 0.2, 0.8) alternate infinite;
  border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
}
</style>
