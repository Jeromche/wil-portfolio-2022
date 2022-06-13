<template>
  <header>
    <h1>Wil van der Tuin</h1>
    <ul>
      <li><a href="#">About</a></li>
      <li><a href="#">Hire me</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
    <div class="avatar">
      <figure>
        <img src="/src/assets/avatar.jpg" />
      </figure>
    </div>
  </header>
</template>

<style scoped>
@keyframes blink {
  0% {
    opacity: 1;
  }

  100% {
    opacity: 0;
  }
}

header {
  display: flex;
  align-items: center;
}

h1 {
  font-family: 'Permanent Marker', cursive;
}

ul {
  --underline-height: 4px;

  display: flex;
  flex-direction: row;
  line-height: 1;
  transform: translateY(var(--underline-height));
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
  inset: 0;
  top: unset;
  width: 0;
  height: var(--underline-height);
  background-color: white;
  transform: translateY(6px);
  transition: width .2s ease-out;
}

a:hover::after {
  width: 100%;
}

a:focus::after {
  width: 100%;
  animation: blink .25s linear;
  animation-iteration-count: 3;
}

.avatar {
  order: 1;
}

figure {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  overflow: hidden;
  border: 1px solid #808080;
}

@media (max-width: 767px) {
  header {
    flex-direction: column;
    place-items: center;
    gap: 16px;
    align-self: center;
    max-width: 320px;
  }

  h1 {
    font-size: 24px;
    order: 2;
  }

  ul {
    order: 3;
    align-self: stretch;
    justify-content: space-between;
    font-size: 14px;
  }
}

@media (min-width: 768px) {
  header {
    flex-direction: row;
    gap: 40px;
  }

  h1 {
    order: 1;
    flex-grow: 1;
    font-size: 32px;
  }

  ul {
    order: 2;
    font-size: 20px;
    gap: 40px;
  }

  .avatar {
    order: 3;
  }
}
</style>
