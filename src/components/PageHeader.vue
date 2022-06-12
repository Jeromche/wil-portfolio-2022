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
  transform: translateY(4px);
}

a {
  display: inline-block;
  color: white;
  text-decoration: none;
  transition: border-bottom-color .1s linear;
  position: relative;
}

a::after {
  content: '';
  position: absolute;
  left: 0;
  right: 0;
  bottom: 0;
  width: 0;
  height: 4px;
  background-color: white;
  transform: translateY(6px);
  transition: width .2s ease-out;
}

a:hover::after {
  width: 100%;
}

figure {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  overflow: hidden;
  border: 1px solid #808080;
}
</style>
