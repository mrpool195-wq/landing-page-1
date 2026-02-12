<template>
    <NavBar />

    <div class="backround-hero pt-6 pb-6">
        <div class="contenedor flex gap-8">
            <div class=" w-1/2 grid place-items-center">
                <h1 class=" text-white h1-hero w-150  ">TECNOLOGIAS INTEGRALES DE
                    COMPUTACION DEL MAYAB
                    SA DE CV</h1>
            </div>
            <div class="w-1/2">
                <img src="../assets/img/compu1.jpg" class="w-150" alt="">
            </div>
        </div>

    </div>

    <section class="section">
        <div class="contenedor flex gap-8">
            <div class="w-1/2">
                <img src="../assets/img/compu1.jpg" alt="" class="w-100">
            </div>
            <div class="w-1/2">
                <h3 class="h3-mision">Nuestra mision</h3>
                <p>
                    Promoveer la transformación digital de las organizaciones mediante el desarrollo, implementación y
                    soporte integral de soluciones tecnológicas innovadoras. Ofrecemos servicios especializados
                    adaptados a las necesidades específicas de cada cliente, garantizando funcionalidad, confiabilidad y
                    continuidad operativa que potencien su productividad y competitividad en el entorno digital.
                </p>
            </div>
        </div>
    </section>

    <section class="section">
        <div class="contenedor flex gap-8">
            <div class="w-1/2">
                <h3 class="h3-mision">Nuestra mision</h3>
                <p>
                    Promoveer la transformación digital de las organizaciones mediante el desarrollo, implementación y
                    soporte integral de soluciones tecnológicas innovadoras. Ofrecemos servicios especializados
                    adaptados a las necesidades específicas de cada cliente, garantizando funcionalidad, confiabilidad y
                    continuidad operativa que potencien su productividad y competitividad en el entorno digital.
                </p>
            </div>
            <div class="w-1/2">
                <img src="../assets/img/compu1.jpg" alt="" class="w-100">
            </div>
        </div>
    </section>

</template>

<style scoped>
.h1-hero {
    font-size: 45px;
    font-weight: bold;
    text-align: left;
}

.backround-hero {
    background-color: var(--color-acento);
}

.h3-mision {
    font-size: 35px;
    padding-bottom: 15px;
    font-weight: 900;
}
</style>

<script>
export default {
    name: 'HomeView',
}
</script>

<script setup>
import NavBar from '@/components/layout/NavBar.vue';
</script>