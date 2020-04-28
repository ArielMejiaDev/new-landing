<template>
    
    <div class="h-screen relative" style="background: url('../assets/images/bg-hero.jpeg');background-position: center;background-repeat: no-repeat; background-size: cover;">

        <!-- overlay -->
        <div class="absolute inset-0 bg-black opacity-50 z-0"></div>

        <Navbar />

        <HeroCallToAction />

    </div>

</template>

<script>
import Navbar from './Navbar'
import HeroCallToAction from './HeroCallToAction'
export default {
    name: 'Hero',
    components: {
        Navbar,
        HeroCallToAction
    }
}
</script>

<style>

</style>