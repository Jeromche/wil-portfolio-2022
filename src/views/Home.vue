<script setup lang="ts">
import Main from '@/components/Main.vue'
import Animation from '@/components/Animation.vue';
import PageHeader from "@/components/PageHeader.vue"
import Hero from '@/components/Hero.vue';
import RecentWork from '@/components/RecentWork.vue';
import Resources from '@/components/Resources.vue';
import Footer from '@/components/Footer.vue';
import AboutMe from '@/components/AboutMe.vue';
</script>

<template>
  <Main>
    <Animation />
    <PageHeader />
    <Hero />
    <RecentWork />
    <Resources />
  </Main>
  <Footer>
    <AboutMe />
  </Footer>
</template>
