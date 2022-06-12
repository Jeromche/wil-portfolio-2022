<template>
  <header>
    <h1>Wil van der Tuin</h1>
    <ul>
      <li><a href="#">About</a></li>
      <li><a href="#">Hire me</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
    <figure>
      <img src="/src/assets/avatar.jpg" />
    </figure>
  </header>
</template>

<style scoped>
header {
  display: flex;
  flex-direction: row;
  place-items: center;
  gap: 40px;
}

h1 {
  font-family: 'Permanent Marker', cursive;
  font-size: 32px;
  flex-grow: 1;
}

ul {
  display: flex;
  flex-direction: row;
  gap: 40px;
  font-size: 20px;
  line-height: 1;
}

a {
  display: inline-block;
  color: white;
  text-decoration: none;
  border-bottom: 2px solid transparent;
  transition: border-bottom-color .1s linear;
}

a:hover {
  border-bottom: 2px solid white;
}

figure {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  overflow: hidden;
  border: 1px solid #808080;
}
</style>
