<template>
    <section>
        <div class="contenedor pt-[100px] pb-[100px]">
            <h2 class="font-bold">Nuestros <span class="text-(--color-valores)">Servicios</span></h2>
            <h3 class="text-center">lo que mejor hacemos</h3>
            <p class="text-center text-gray-400">Ofrecemos soluciones integrales que cubren todo el espectro
                tecnológico.
            </p>
            <div class="servicios-cards mt-6">
                <CardService title="Desarrollo a Medida"
                    info="Aplicaciones web y móviles construidas con las últimas tecnologías y mejores prácticas." />

                <CardService title="Desarrollo a Medida"
                    info="Aplicaciones web y móviles construidas con las últimas tecnologías y mejores prácticas." />

                <CardService title="Desarrollo a Medida"
                    info="Aplicaciones web y móviles construidas con las últimas tecnologías y mejores prácticas." />
                <CardService title="Desarrollo a Medida"
                    info="Aplicaciones web y móviles construidas con las últimas tecnologías y mejores prácticas." />

                <CardService title="Desarrollo a Medida"
                    info="Aplicaciones web y móviles construidas con las últimas tecnologías y mejores prácticas." />

                <CardService title="Desarrollo a Medida"
                    info="Aplicaciones web y móviles construidas con las últimas tecnologías y mejores prácticas." />
            </div>
        </div>
    </section>
</template>

<style>
.contenedor h2 {
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
</script>
