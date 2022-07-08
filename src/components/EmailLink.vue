<script lang="ts" setup>
</script>

<template>
  <a href="mailto:wil@vandertuin.nl">
    <span class="address">wil@vandertuin.nl</span>
    <svg width="2" height="23" viewBox="0 0 2 23" fill="none" xmlns="http://www.w3.org/2000/svg">
      <line x1="0.75" y1="3.27835e-08" x2="0.749999" y2="23" stroke="#070095" stroke-width="1.5"
        stroke-dasharray="3 3" />
    </svg>
    <span class="copy">
      <span class="button">
        <svg width="18" height="19" viewBox="0 0 18 19" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path
            d="M15 7.25H8.25C7.42157 7.25 6.75 7.92157 6.75 8.75V15.5C6.75 16.3284 7.42157 17 8.25 17H15C15.8284 17 16.5 16.3284 16.5 15.5V8.75C16.5 7.92157 15.8284 7.25 15 7.25Z"
            stroke="#070095" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
          <path
            d="M3.75 11.75H3C2.60218 11.75 2.22064 11.592 1.93934 11.3107C1.65804 11.0294 1.5 10.6478 1.5 10.25V3.5C1.5 3.10218 1.65804 2.72064 1.93934 2.43934C2.22064 2.15804 2.60218 2 3 2H9.75C10.1478 2 10.5294 2.15804 10.8107 2.43934C11.092 2.72064 11.25 3.10218 11.25 3.5V4.25"
            stroke="#070095" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
        </svg>
      </span>
    </span>
  </a>
</template>

<style scoped>
a {
  --blue: #070095;
  --white: #E0DFFF;

  background-color: var(--white);
  color: var(--blue);
  display: inline-flex;
  flex-direction: row;
  align-items: center;
  padding-block: 12px;
  border-radius: 2px;
  box-shadow: 5px 5px 0 #070095;
  text-decoration: none;
  position: relative;
  z-index: 1;
}

.address {
  padding-left: 24px;
  padding-right: 22px;
  font-size: 18px;
  font-weight: 500;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

.copy {
  padding-left: 18px;
  padding-right: 20px;
}

.button {
  position: relative;
  z-index: 2;
  border-radius: 4px;
  padding: 4px;
  display: block;
  transition: background-color .5s ease-out;
}

.button path {
  transition: stroke .25s ease-out;
}

.button:hover {
  background-color: var(--blue);
}

.button:hover path {
  stroke: var(--white);
}
</style>
