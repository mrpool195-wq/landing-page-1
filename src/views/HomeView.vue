<template>
    <NavBar />

    <HeroSectionView />

    <ServicioSection />
    <StatsSection />
    <PricingSection />



    <FooTer />
</template>

<script>
export default {
    name: 'HomeView',
}
</script>

<script setup>
import FooTer from '@/components/layout/FooTer.vue';
import NavBar from '@/components/layout/NavBar.vue';
import HeroSectionView from '@/components/sections/HeroSectionView.vue';
import PricingSection from '@/components/sections/PricingSection.vue';
import ServicioSection from '@/components/sections/ServicioSection.vue';
import StatsSection from '@/components/sections/StatsSection.vue';
</script>