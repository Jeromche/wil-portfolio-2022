<template>
  <router-view />
</template>

<style>
@import '/node_modules/modern-normalize/modern-normalize.css';

body {
  background-color: hsl(0, 0%, 14%);
  color: white;
  font-family: 'Poppins', sans-serif;
  padding-inline: 40px;
  padding-block: 60px;
}

#app {
  display: flex;
  flex-direction: column;
  gap: 400px;
  max-width: 1080px;
  margin: 0 auto;
}
</style>
