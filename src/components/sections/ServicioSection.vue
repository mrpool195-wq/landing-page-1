<template>
    <section>
        <div class="contenedor contenedor-servicios pt-[100px] pb-[100px]">
            <h2 class="font-bold">Nuestros <span class="text-(--color-valores)">Servicios</span></h2>
            <h3 class="text-center">lo que mejor hacemos</h3>
            <p class="text-center text-gray-400">Servicios de consultoría en computación </p>
            <div class="servicios-cards mt-6">
                <CardService :icon="CodeBracketIcon" title="Desarrollo a Medida"
                    info="Aplicaciones web y móviles construidas con las últimas tecnologías y mejores prácticas." />

                <CardService :icon="CloudIcon" title="Infraestructura Cloud"
                    info="Arquitectura escalable y resiliente en la nube para tu negocio." />

                <CardService :icon="ShieldCheckIcon" title="Ciberseguridad"
                    info="Protección avanzada de datos y sistemas contra amenazas digitales." />
                <CardService :icon="CpuChipIcon" title="Inteligencia Artificial"
                    info="Soluciones de IA y machine learning que automatizan y optimizan procesos." />

                <CardService :icon="ChartBarIcon" title="Análisis de Datos"
                    info="Transformamos datos en insights accionables para la toma de decisiones." />

                <CardService :icon="DevicePhoneMobileIcon" title="Apps Móviles"
                    info="Experiencias móviles nativas y multiplataforma de alto rendimiento." />
            </div>
        </div>
    </section>
</template>

<style>
.contenedor-servicios h2 {
    font-size: 40px;
    text-align: center;
}

.contenedor h3 {
    font-size: 22px;
    padding-bottom: 10px;
}

.servicios-cards {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}
</style>

<script setup>
import CardService from '../ui/CardService.vue';
import { CodeBracketIcon } from '@heroicons/vue/24/solid';
import { CloudIcon } from '@heroicons/vue/24/solid';
import { ShieldCheckIcon } from '@heroicons/vue/24/solid';
import { CpuChipIcon } from '@heroicons/vue/24/solid';
import { ChartBarIcon } from '@heroicons/vue/24/solid';
import { DevicePhoneMobileIcon } from '@heroicons/vue/24/solid';


</script>
