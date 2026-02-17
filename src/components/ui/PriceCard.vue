<template>
    <div class="tarjeta-precio border border-gray-300 w-1/4 rounded-[20px] py-6 px-4"
        :class="{ 'bg-gradient-to-t from-[#983dff] to-texto': popular }">
        <!-- <span v-if="popular" class="badge">El más vendido</span> -->
        <div class="pb-[20px]" :class="{ 'flex align-middle justify-between': popular }">
            <h2 class="align-middle">{{ titulo_plan }}</h2>
            <span v-if="popular"
                class="flex gap-2 border rounded-[20px] py-[5px] px-[15px] text-(--texto) bg-gradient-to-bl from-[#983dff]">
                <StarIcon class="w-5" />
                Popular
            </span>
        </div>
        <p>{{ descripcion_plan }}</p>
        <span class="text-[25px] pb-[20px]">{{ precio }}</span>
        <ul>
            <li v-for="(item, index) in caracteristicas" :key="index">
                <div class="flex gap-2 pt-4">
                    <div class="w-8 h-8">
                        <CheckCircleIcon class="w-full h-full text-(--color-vibrante)"
                            :class="{ 'text-(--texto)': popular }" />
                    </div>
                    {{ item }}
                </div>
            </li>
        </ul>
    </div>
</template>

<style>
.tarjeta-precio span {
    font-weight: bold;
}

.tarjeta-precio h2 {
    font-weight: bold;
}

.tarjeta-precio p {
    padding-bottom: 20px;
}
</style>

<script setup>
defineProps({
    titulo_plan: String,
    descripcion_plan: String,
    precio: String,
    popular: {
        type: Boolean,
        default: false
    },
    caracteristicas: Array
})

import { CheckCircleIcon } from '@heroicons/vue/24/solid';
import { StarIcon } from '@heroicons/vue/24/solid';


</script>
