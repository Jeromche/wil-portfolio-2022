<template>
  <article>
    <figure />
    <div>
      <h3>A toggle switch</h3>
      <p>An accessible switch that falls back to a checkbox.</p>
    </div>
  </article>
</template>

<style scoped>
article {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

figure {
  height: 142px;
  background-color: #D9D9D9;
}

div {
  display: flex;
  flex-direction: column;
  gap: 4px;
  line-height: 1.5;
}

h3 {
  font-weight: 500;
  font-size: 16px;
}

p {
  font-weight: 400;
  font-size: 14px;
}
</style>
