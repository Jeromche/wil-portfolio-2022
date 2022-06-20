<template>
  <section>
    <h2>About me</h2>
    <div class="container">
      <div class="content">
        <p>I was born in The Netherlands in the eighties. Ever since I was young kid I was interested in computers and I
          always knew I was going to be a programmer. In my teens I learned how to create websites with HTML and when I
          was 18 years old I started my first job at a local web agency and I've been slinging code ever since.</p>
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
