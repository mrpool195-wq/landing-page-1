<script setup lang="ts">
import PriceCard from '../ui/PriceCard.vue';

</script>

<template>
    <section class="section">
        <div class="contenedor ">
            <h2 class="text-[40px] font-bold text-center">Nuestros <span class="text-(--color-valores)">Precios</span>
            </h2>
            <div class="flex gap-8 justify-center my-[90px] ">
                <PriceCard titulo_plan="Basic pack"
                    descripcion_plan="So I started to walk into the water. I won't lie to you boys, I was terrified. B"
                    precio="$ 999/mes" :caracteristicas="[
                        'Soporte 24/7',
                        'Panel avanzado',
                        'Backups automáticos',
                        'asd'
                    ]" />
                <PriceCard titulo_plan="Pro pack"
                    descripcion_plan="So I started to walk into the water. I won't lie to you boys, I was terrified. B"
                    precio="$ 999/mes" :popular="true" :caracteristicas="[
                        'Soporte 24/7',
                        'Panel avanzado',
                        'Backups automáticos',
                        'asd',
                        'Soporte 24/7',
                        'Panel avanzado',
                        'Backups automáticos',
                    ]" />
                <PriceCard titulo_plan="Enterprise pack"
                    descripcion_plan="So I started to walk into the water. I won't lie to you boys, I was terrified. B"
                    precio="$ 999/mes" :caracteristicas="[
                        'Soporte 24/7',
                        'Panel avanzado',
                        'Backups automáticos',
                        'asd',
                        'Soporte 24/7',
                        'Panel avanzado',
                        'Backups automáticos',
                        'asd',
                        'Soporte 24/7',
                        'Panel avanzado',
                    ]" />
            </div>
        </div>
    </section>
</template>