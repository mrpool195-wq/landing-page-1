<template>
    <div class="tarjeta-servicio border p-6 rounded-xl border border-gray-300 w-100">
        <h3 class="font-bold pb-4">{{ title }}</h3>
        <p class="text-gray-400">{{ info }}</p>
    </div>
</template>

<script setup>
defineProps({
    title: String,
    info: String
})
</script>

<style></style>