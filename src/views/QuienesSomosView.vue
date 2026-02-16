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
        <div class="contenedor flex gap-[10vw] justify-center contenedor-mision">
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

    <section class="section bg-(--texto)">
        <div class="contenedor">
            <div class="valores-container p-4">
                <h2 class="">Nuestros Valores</h2>
                <div class="p-6 flex gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4">
                    <div
                        class="elemento-valor bg-(--color-valores) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <h4>1</h4>
                    </div>
                    <div>
                        <h3>Proactividad</h3>
                        <p>Anticipamos las necesidades tecnológicas de nuestros clientes antes de que se conviertan en
                            problemas
                            críticos. Monitoreamos constantemente el rendimiento de los sistemas, identificamos
                            oportunidades de
                            mejora y recomendamos actualizaciones o soluciones preventivas que optimicen la
                            infraestructura
                            tecnológica y eviten interrupciones en las operaciones del negocio.</p>
                    </div>
                </div>

                <div class="p-6 flex gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4">
                    <div
                        class="elemento-valor bg-(--color-valores) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <h4>2</h4>
                    </div>
                    <div>
                        <h3>Colaboración</h3>
                        <p>Trabajamos en estrecha alianza con nuestros clientes, construyendo relaciones basadas en la
                            comunicación abierta y el trabajo en equipo. Entendemos que el éxito tecnológico requiere la
                            participación activa de ambas partes, por lo que fomentamos el intercambio de conocimientos,
                            la
                            capacitación y la co-creación de soluciones que realmente respondan a sus desafíos
                            operativos.</p>
                    </div>
                </div>

                <div class="p-6 flex gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4">
                    <div
                        class="elemento-valor bg-(--color-valores) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <h4>3</h4>
                    </div>
                    <div>
                        <h3>Eficiencia</h3>
                        <p>Optimizamos recursos, tiempos y procesos para entregar soluciones tecnológicas que maximicen
                            el
                            retorno de inversión de nuestros clientes. Diseñamos arquitecturas tecnológicas escalables y
                            sostenibles, automatizamos procesos repetitivos y garantizamos que cada implementación
                            genere
                            mejoras medibles en productividad y reducción de costos operativos.</p>
                    </div>
                </div>

                <div class="p-6 flex gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4">
                    <div
                        class="elemento-valor bg-(--color-valores) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <h4>4</h4>
                    </div>
                    <div>
                        <h3>Seguridad</h3>
                        <p>Priorizamos la protección de la información y los activos digitales de nuestros clientes en
                            cada
                            solución que desarrollamos. Implementamos las mejores prácticas de ciberseguridad, cumplimos
                            con
                            estándares internacionales de protección de datos y diseñamos sistemas resilientes que
                            salvaguarden
                            la integridad, confidencialidad y disponibilidad de la información crítica del negocio.</p>
                    </div>
                </div>

                <div class="p-6 flex gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4">
                    <div
                        class="elemento-valor bg-(--color-valores) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <h4>5</h4>
                    </div>
                    <div>
                        <h3>Responsabilidad</h3>
                        <p>Asumimos plena accountability por el impacto y funcionamiento de las soluciones tecnológicas
                            que
                            entregamos. Documentamos adecuadamente cada implementación, brindamos soporte continuo
                            post-venta,
                            atendemos incidencias con urgencia y nos hacemos cargo de resolver cualquier problema
                            derivado de
                            nuestros servicios hasta la completa satisfacción del cliente</p>
                    </div>
                </div>







            </div>
        </div>
    </section>
</template>

<style scoped>
.card-valor {
    background-color: var(--color-acento);
}

.contenido-valores {
    background-color: var(--color-valores);
}

/* .valores-container {} */

.valores-container h2 {
    font-size: 43px;
    text-align: center;
    padding-bottom: 40px;
    color: var(--color-valores);
    font-weight: bold;
}

.valores-container h3 {
    font-size: 20px;
    font-weight: bold;
    padding-bottom: 20px;
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

    .contenedor-mision {
        display: flex;
        flex-direction: column-reverse;
        text-align: center;
        align-items: center;
    }

    .contenedor-mision div {
        width: 100%;
        padding: 40px;
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
</script>
