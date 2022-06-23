<template>
  <section>
    <h2>About me</h2>
    <div class="container">
      <div class="content">
        <p>I am a T-shaped engineer with strong expertise in the web platform (site optimization, accessibility,
          useability) with Vuejs and React. Besides my specialty as a UI engineer I have experience in multiple
          supporting areas such as infrastructure, database design, Node backend, marketing, A/B testing, UI wireframing
          and design.</p>
      </div>
      <div class="items" />
    </div>
  </section>
</template>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  gap: 24px;
}

h2 {
  font-family: 'Permanent Marker', cursive;
  font-size: 20px;
  line-height: 1.5;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 36px;
}

.content {
  font-weight: 400;
  font-size: 16px;
  line-height: 1.5;
  padding-right: 100px;
}

.content p {
  margin-bottom: 1em;
}

.items {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 36px;
}
</style>
