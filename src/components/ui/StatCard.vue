<template>
    <div class="border w-1/2">
        <h2 class="">{{ valor }}</h2>
        <p class="text-center">{{ description }}</p>
    </div>
</template>

<script setup>
defineProps({
    valor: String,
    description: String
})
</script>