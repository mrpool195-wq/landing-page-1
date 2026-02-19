<template>

    <!-- <div class="backround-hero pt-[100px] pb-[100px]"> -->
    <div class="relative bg-[url(/src/assets/img/tech4.jpg)] bg-cover bg-center pt-[100px] pb-[100px]">
        <div
            class="pointer-events-none absolute inset-0 bg-gradient-to-r from-[var(--color-pricipal)] from-0% via-[var(--color-pricipal)] via-40% to-transparent to-100%">
        </div>

        <div class="contenedor hero relative z-10 flex gap-8">
            <div class="w-1/2">
                <h1 class=" text-white h1-hero">Impulsando tu transformación digital</h1>
                <h2 class="text-(--subtitulos) !text-[40px] font-bold">Tecnologia Innovadora</h2>
                <p class="text-white pt-4">Convertimos ideas en soluciones tecnológicas escalables que optimizan
                    procesos,
                    aumentan tu
                    competitividad y preparan tu negocio para el futuro.</p>
                <div class="pt-8 flex gap-6">
                    <a href=""
                        class="bg-(--color-boton1) inline-block py-4 px-8 rounded-md font-semibold !text-[14px] text-(--blanco1) transition-shadow duration-300 hover:shadow-[0_0_16px_#dddddd]">Conoce
                        más
                    </a>
                    <a href=""
                        class="bg-(--blanco1) inline-block py-4 px-8 rounded-md font-semibold !text-[14px] transition-shadow duration-300 hover:shadow-[0_0_16px_#dddddd]">Contactanos
                    </a>
                </div>
            </div>

            <div class="w-1/2">
                <!-- <img src="/src/assets/img/compu1.jpg" class="w-150 rounded-xl" alt=""> -->
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
