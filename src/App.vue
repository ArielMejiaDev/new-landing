<template>
  <div id="app" class="font-body">
    <Hero />
    <StepsSection />
  </div>
</template>

<script>
import Hero from './components/Hero'
import StepsSection from './components/StepsSection'
export default {
  name: 'App',
  components: {
    Hero,
    StepsSection,
  }
}
</script>

<style lang="scss">
</style>
