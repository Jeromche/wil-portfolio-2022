<script lang="ts" setup>
import ResourceItem from './ResourceItem.vue';
</script>

<template>
  <section>
    <h2>Resources</h2>
    <div class="container">
      <div class="content">
        <p>Every now and again I create components or widgets on Codepen to experiment how I would make something, to
          learn how to create the best version or just to pass the time.</p>
        <p>Here is a selection list of what I've been up to lately. Feel free to copy and use any of it in your own
          projects.
        </p>
      </div>
      <div class="items">
        <ResourceItem />
        <ResourceItem />
        <ResourceItem />
        <ResourceItem />
        <ResourceItem />
      </div>
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
