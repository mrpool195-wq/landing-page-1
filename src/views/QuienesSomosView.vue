<template>
    <NavBar />
    <div class="backround-hero pt-[100px] pb-[100px]">
        <div class="contenedor hero">
            <div class="grid place-items-center">
                <h1 class=" text-white h1-hero">Quienes somos</h1>
            </div>
        </div>
    </div>
    <section class="section">
        <div class="contenedor flex gap-[10vw] justify-center">
            <div class="w-1/2">
                <img src="../assets/img/compu1.jpg" alt="" class="rounded-[40px]">
            </div>
            <div class="w-1/2">
                <h3 class="h3-mision">Mision</h3>
                <p class="text-gray-500 text-justify pt-[30px]">
                    Promoveer la transformación digital de las organizaciones mediante el desarrollo, implementación y
                    soporte integral de soluciones tecnológicas innovadoras. Ofrecemos servicios especializados
                    adaptados a las necesidades específicas de cada cliente, garantizando funcionalidad, confiabilidad y
                    continuidad operativa que potencien su productividad y competitividad en el entorno digital.
                </p>
            </div>
        </div>
    </section>

    <section class="section section-bg">
        <VisionSectionView />
    </section>

    <section class="section">
        <div class="contenedor contenido-valoress">
            <div class="card-valor border rounded-[20px] p-4 flex gap-8">
                <div class="bg-blue-500 w-100">
                    <iconMenu />
                </div>
                <div>
                    <h4 class="font-[1000] text-[25px] pb-4">Proactividad</h4>
                    <p>Anticipamos las necesidades tecnológicas de nuestros clientes antes de que se conviertan en
                        problemas críticos. Monitoreamos constantemente el rendimiento de los sistemas, identificamos
                        oportunidades de mejora y recomendamos actualizaciones o soluciones preventivas que optimicen la
                        infraestructura tecnológica y eviten interrupciones en las operaciones del negocio.</p>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.contenido-valores {
    background-color: var(--color-valores);
}

.h1-hero {
    font-size: 45px;
    font-weight: bold;
    text-align: center;
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
<script>

export default {
    name: 'QuienesSomosView',
}
</script>
<script setup>
import NavBar from '@/components/layout/NavBar.vue';
import VisionSectionView from '@/components/sections/VisionSectionView.vue';
import iconMenu from '@/components/icons/iconMenu.vue';
</script>