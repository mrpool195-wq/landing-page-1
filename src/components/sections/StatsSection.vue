<template>
    <section class="section relative bg-[url(/src/assets/img/tec3.jpg)] bg-fixed bg-center">
        <!-- Overlay/filtro -->
        <div class="absolute inset-0 bg-[#543676]/60"></div>

        <!-- Contenido por encima -->
        <div class="contenedor relative z-10 flex items-center justify-center gap-[10vw]">
            <StatCard valor="150+" description="PROYECTOS ENTREGADOS" />
            <StatCard valor="99.9%" description="PROYECTOS ENTREGADOS" />
            <StatCard valor="50+" description="PROYECTOS ENTREGADOS" />
            <StatCard valor="24/7" description="PROYECTOS ENTREGADOS" />
        </div>
    </section>
</template>
<script setup>
import StatCard from '../ui/StatCard.vue';
</script>