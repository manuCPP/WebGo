<script setup>
import { RouterLink, RouterView } from 'vue-router'
import NavBar from './components/NavBar.vue'
import Hero from './components/sections/Hero.vue'
import BulletSection from '@/components/sections/BulletSection.vue'
import Spacers from '@/components/Spacer.vue'
import PricesSection from '@/components/sections/PricesSection.vue'

</script>

<template>
  <NavBar/>
  <Hero/>
  <Spacers space="8"/>
  <BulletSection/>
  <PricesSection/>
</template>

<style scoped>

</style>
