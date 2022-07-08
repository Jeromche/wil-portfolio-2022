<script lang="ts" setup>
import EmailLink from '@/components/EmailLink.vue';
</script>

<template>
  <section>
    <article>
      <div>
        <h2>About me</h2>
        <p>I work with the web platform (site optimization, accessibility, useability) with Vuejs and React. Besides my
          specialty as a UI engineer I have experience in multiple supporting areas such as infrastructure, database
          design, Node backend, marketing, A/B testing, UI wireframing and design.</p>
      </div>
      <div>
        <h2>Hire me</h2>
        <p>If you think I could make a positive impact at your organization then please get in touch with me.</p>
      </div>
      <div>
        <EmailLink />
      </div>
    </article>
  </section>
</template>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  gap: 24px;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.5;
}

article {
  display: flex;
  flex-direction: column;
  gap: 64px;
}

article>div:not(:last-child) {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

h2 {
  font-size: 20px;
  line-height: 1.5;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  font-weight: 500;
  letter-spacing: 0.1;
}

p {
  margin-bottom: 1em;
}

@media (min-width: 768px) {
  section {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 36px;
  }
}
</style>
