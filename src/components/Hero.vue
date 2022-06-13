<script setup lang="ts">
import TitleSlide from '@/components/TitleSlide.vue'
</script>

<template>
  <section>
    <div class="hero">
      <h2 class="desktop">
        <title-slide line="Wil here, creative web developer" />
        <title-slide line="and taco connoiseur 🌮" />
      </h2>
      <p>I love connecting companies with their customers through perfectly implemented, accessible and easy to use web
        interfaces.</p>
    </div>
    <div class="cta">
      <a class="button" href="#">Download CV</a>
      <a class="text" href="mailto:wil@vandertuin.nl">wil@vandertuin.nl</a>
    </div>
  </section>
</template>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  gap: 64px;
}

.hero {
  display: flex;
  flex-direction: column;
  gap: 22px;
  max-width: 800px;
}

h2 {
  font-size: 24px;
  font-weight: 700;
  line-height: 1.3;
}

p {
  font-size: 18px;
  font-weight: 500;
  line-height: 1.5;
}

.cta {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 16px;
}

.cta a {
  display: inline-block;
  color: white;
}

.button {
  background-color: hsl(243, 100%, 66%);
  font-family: 'Permanent Marker', cursive;
  padding: 18px 36px;
  border-radius: 36px;
  text-decoration: none;
  white-space: nowrap;
  font-size: 20px;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  transition: all .15s linear;
  box-shadow: 0 4px 1px transparent;
}

.button:hover {
  background-image: linear-gradient(hsl(243, 100%, 66%), hsl(243, 65%, 55%));
  box-shadow: 0 4px 1px hsl(243deg 61% 42%);
  text-shadow: 1px 2px 0px hsl(243deg 61% 50%);
  transform: translateY(-1px);
}

.button:active {
  transform: translateY(1px);
  box-shadow: 0 2px 0px hsl(243deg 61% 42%);
}

.text {
  font-size: 24px;
}

@media (min-width: 768px) {
  .cta {
    flex-direction: row;
    gap: 40px;
  }
}

@media (min-width: 1024px) {
  h2 {
    font-size: 40px;
  }

  p {
    font-size: 24px;
  }
}
</style>
