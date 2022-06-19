<script setup lang="ts">
interface Props {
  name: string;
  type: string;
}

defineProps<Props>()
</script>

<template>
  <article>
    <figure />
    <header>
      <h3>{{ name }}</h3>
      <h4>{{ type }}</h4>
    </header>
    <div>
      <slot />
    </div>
  </article>
</template>

<style scoped>
article {
  display: flex;
  flex-direction: column;
  gap: 16px;
}

header {
  display: flex;
  flex-direction: row;
  gap: 36px;
  font-weight: 500;
  font-size: 20px;
  line-height: 1.5;
}

div {
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
}

figure {
  background-color: #D9D9D9;
  height: 242px;
}
</style>
