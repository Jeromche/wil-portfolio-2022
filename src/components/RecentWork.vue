<script lang="ts" setup>
import RecentWorkItem from './RecentWorkItem.vue';
</script>

<template>
  <section>
    <h2>Recent Work</h2>
    <div class="container">
      <RecentWorkItem name="Suggestic.com" type="B2B Lead generation site">
        <p>Website that showcases our products, services and technology. We did a complete overhaul of the content of
          our previous website and organized it on the Contentful CMS. The pages are server side generated with Nuxt.js
          and Vue.</p>
      </RecentWorkItem>
      <RecentWorkItem name="Mezcla Viva" type="B2C Lead generation site">
        <p>Website for a landscaping company with custom image browser. Also built with Nuxt.js and hooked up to
          Contenful.</p>
      </RecentWorkItem>
      <RecentWorkItem name="CDMX.gay" type="Domain name sale mini site">
        <p>The day that the .gay TLD became available I snatched up CDMX.gay, the letters of the city where I live,
          Mexico City. Get in touch for a great deal!</p>
      </RecentWorkItem>
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
  grid-template-columns: auto;
  row-gap: 64px;
}

@media (min-width: 768px) {
  .container {
    grid-template-columns: 1fr 1fr;
    column-gap: 36px;
    row-gap: 104px;
  }
}
</style>
