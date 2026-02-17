<template>
    <div class="tarjeta-servicio sw-1/2">
        <h2 class="">{{ valor }}</h2>
        <p class="text-center text-white">{{ description }}</p>
    </div>
</template>
<style>
.tarjeta-servicio h2 {
    font-size: 60px;
    text-align: center;
    font-weight: bold;
    color: var(--texto);
}
</style>

<script setup>
defineProps({
    valor: String,
    description: String
})
</script>