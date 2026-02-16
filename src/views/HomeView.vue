<template>
    <NavBar />

    <HeroSectionView />

    <ServicioSection />
    <StatsSection />




</template>

<script>
export default {
    name: 'HomeView',
}
</script>

<script setup>
import NavBar from '@/components/layout/NavBar.vue';
import HeroSectionView from '@/components/sections/HeroSectionView.vue';
import ServicioSection from '@/components/sections/ServicioSection.vue';
import StatsSection from '@/components/sections/StatsSection.vue';
</script>