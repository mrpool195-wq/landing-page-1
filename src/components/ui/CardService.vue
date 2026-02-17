<template>
    <div class="tarjeta-servicio border p-6 rounded-xl border border-gray-300 w-100">
        <div v-if="icon"
            class="border border-(--color-vibrante) w-10 h-10 p-2 rounded-lg mb-4 text-(--color-vibrante) bg-(--fondo-1)">
            <component :is="icon" class="w-full h-full" />
        </div>
        <h3 class="font-bold pb-4">{{ title }}</h3>
        <p class="text-gray-400">{{ info }}</p>
    </div>
</template>

<script setup>
defineProps({
    title: String,
    info: String,
    icon: Object
})
</script>

<style></style>