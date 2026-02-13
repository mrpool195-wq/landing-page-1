<template>

    <div class="backround-hero pt-[100px] pb-[100px]">
        <div class="contenedor hero flex gap-8">
            <div class="w-1/2 grid place-items-center">
                <h1 class=" text-white h1-hero">Impulsando tu transformación digital</h1>
            </div>
            <div class="w-1/2">
                <img src="/src/assets/img/compu1.jpg" class="w-150 rounded-xl" alt="">
            </div>
        </div>
    </div>
</template>

<style scoped>
.h1-hero {
    font-size: 45px;
    font-weight: bold;
    text-align: left;
}

.backround-hero {
    background-color: var(--color-pricipal);
}



.h3-mision {
    font-size: 55px;
    padding-bottom: 15px;
    font-weight: 900;
}

@media (max-width: 768px) {
    .hero {
        flex-direction: column;
        text-align: center;
        align-items: center;
    }

    .h1-hero {
        font-size: 1.2rem;
        font-weight: bold;
        text-align: center;
    }

}
</style>
