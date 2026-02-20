<template>
    <NavBar />
    <div
        class="bg-(--color-pricipal) bg-[radial-gradient(#4F4E50_1px,transparent_1px)] bg-[size:20px_20px]  pt-[100px] pb-[100px] ">
        <div class="contenedor hero">
            <div class="grid place-items-center">
                <h1 class=" text-white h1-hero">Nosotros</h1>
                <p class="text-(--blanco1) !text-[20px] py-6">Conoce quiénes somos, nuestra misión, visión y los valores
                    que
                    guían cada
                    proyecto que emprendemos.
                </p>
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
        <!-- <div
            class="w-1/2 bg-transparent bg-[radial-gradient(var(--color-pricipal),transparent_1px)] bg-[size:20px_20px] h-100">

        </div> -->
    </section>

    <section class="section bg-(--subtitulos)">
        <VisionSectionView />
    </section>

    <section class="section">
        <div class="contenedor">
            <h2 class="">Nuestros Valores</h2>
            <div class="valores-container p-4 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">

                <div class="relative p-6 gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4 ">
                    <div
                        class="elemento-valor absolute top-[-30px] left-[-30px] bg-(--color-pricipal) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                            <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                stroke-width="2">
                                <path
                                    d="M4 13a8 8 0 0 1 7 7a6 6 0 0 0 3-5a9 9 0 0 0 6-8a3 3 0 0 0-3-3a9 9 0 0 0-8 6a6 6 0 0 0-5 3" />
                                <path d="M7 14a6 6 0 0 0-3 6a6 6 0 0 0 6-3m4-8a1 1 0 1 0 2 0a1 1 0 1 0-2 0" />
                            </g>
                        </svg>
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

                <div class="relative p-6 gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4 ">
                    <div
                        class="elemento-valor absolute top-[-30px] left-[-30px] bg-(--color-pricipal) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 14 14">
                            <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round">
                                <path
                                    d="M12.5.5h-11a1 1 0 0 0-1 1v11a1 1 0 0 0 1 1h11a1 1 0 0 0 1-1v-11a1 1 0 0 0-1-1" />
                                <path d="M7 .5v2.132a1.5 1.5 0 1 0 0 2.236v4.264a1.5 1.5 0 1 1 0 2.236V13.5" />
                                <path d="M.5 7h2.132a1.5 1.5 0 1 0 2.236 0h4.264a1.5 1.5 0 1 1 2.236 0H13.5" />
                            </g>
                        </svg>
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

                <div class="relative p-6 gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4 ">
                    <div
                        class="elemento-valor absolute top-[-30px] left-[-30px] bg-(--color-pricipal) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                            <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                stroke-width="2">
                                <path
                                    d="M4 13a8 8 0 0 1 7 7a6 6 0 0 0 3-5a9 9 0 0 0 6-8a3 3 0 0 0-3-3a9 9 0 0 0-8 6a6 6 0 0 0-5 3" />
                                <path d="M7 14a6 6 0 0 0-3 6a6 6 0 0 0 6-3m4-8a1 1 0 1 0 2 0a1 1 0 1 0-2 0" />
                            </g>
                        </svg>
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

                <div class="relative p-6 gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4 ">
                    <div
                        class="elemento-valor absolute top-[-30px] left-[-30px] bg-(--color-pricipal) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                            <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                stroke-width="2">
                                <path
                                    d="M4 13a8 8 0 0 1 7 7a6 6 0 0 0 3-5a9 9 0 0 0 6-8a3 3 0 0 0-3-3a9 9 0 0 0-8 6a6 6 0 0 0-5 3" />
                                <path d="M7 14a6 6 0 0 0-3 6a6 6 0 0 0 6-3m4-8a1 1 0 1 0 2 0a1 1 0 1 0-2 0" />
                            </g>
                        </svg>
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

                <div class="relative p-6 gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4 ">
                    <div
                        class="elemento-valor absolute top-[-30px] left-[-30px] bg-(--color-pricipal) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                            <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                stroke-width="2">
                                <path
                                    d="M4 13a8 8 0 0 1 7 7a6 6 0 0 0 3-5a9 9 0 0 0 6-8a3 3 0 0 0-3-3a9 9 0 0 0-8 6a6 6 0 0 0-5 3" />
                                <path d="M7 14a6 6 0 0 0-3 6a6 6 0 0 0 6-3m4-8a1 1 0 1 0 2 0a1 1 0 1 0-2 0" />
                            </g>
                        </svg>
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


                <!-- <div class="p-6 flex gap-8 border border-(--color-neutro) rounded-xl bg-(--color-neutro) mt-4">
                    <div
                        class="elemento-valor bg-(--color-pricipal) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 14 14">
                            <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round">
                                <path
                                    d="M12.5.5h-11a1 1 0 0 0-1 1v11a1 1 0 0 0 1 1h11a1 1 0 0 0 1-1v-11a1 1 0 0 0-1-1" />
                                <path d="M7 .5v2.132a1.5 1.5 0 1 0 0 2.236v4.264a1.5 1.5 0 1 1 0 2.236V13.5" />
                                <path d="M.5 7h2.132a1.5 1.5 0 1 0 2.236 0h4.264a1.5 1.5 0 1 1 2.236 0H13.5" />
                            </g>
                        </svg>
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
                        class="elemento-valor bg-(--color-pricipal) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                            <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                stroke-width="2"
                                d="M17.684 3.603c.521-.659.03-1.603-.836-1.603h-6.716a1.06 1.06 0 0 0-.909.502l-5.082 8.456c-.401.666.103 1.497.908 1.497h3.429l-3.23 8.065c-.467 1.02.795 1.953 1.643 1.215L20 9.331h-6.849z" />
                        </svg>
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
                        class="elemento-valor bg-(--color-pricipal) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                            <g fill="none">
                                <path d="M3 4.65V12c0 7.35 9 10.5 9 10.5s9-3.15 9-10.5V4.65L12 1.5z"
                                    clip-rule="evenodd" />
                                <path stroke="currentColor" stroke-linecap="square" stroke-width="2"
                                    d="M3 4.65V12c0 7.35 9 10.5 9 10.5s9-3.15 9-10.5V4.65L12 1.5z"
                                    clip-rule="evenodd" />
                                <path stroke="currentColor" stroke-linecap="square" stroke-width="2"
                                    d="M8.173 11.172L11 14l5.657-5.657" />
                            </g>
                        </svg>
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
                        class="elemento-valor bg-(--color-pricipal) text-white rounded-full w-15 h-15 flex items-center justify-center flex-shrink-0">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                            <path fill="currentColor"
                                d="M12.75 2.75V4.5h1.975c.351 0 .694.106.984.303l1.697 1.154q.063.042.14.043h4.102a.75.75 0 0 1 0 1.5H20.07l3.366 7.68a.75.75 0 0 1-.23.896q-.15.111-.31.206a6 6 0 0 1-.79.399a7.35 7.35 0 0 1-2.856.569a7.3 7.3 0 0 1-2.855-.568a6 6 0 0 1-.79-.4a3 3 0 0 1-.307-.202l-.005-.004a.75.75 0 0 1-.23-.896l3.368-7.68h-.886c-.351 0-.694-.106-.984-.303l-1.697-1.154a.25.25 0 0 0-.14-.043H12.75v14.5h4.487a.75.75 0 0 1 0 1.5H6.763a.75.75 0 0 1 0-1.5h4.487V6H9.275a.25.25 0 0 0-.14.043L7.439 7.197c-.29.197-.633.303-.984.303h-.886l3.368 7.68a.75.75 0 0 1-.209.878c-.08.065-.16.126-.31.223a6 6 0 0 1-.792.433a6.9 6.9 0 0 1-2.876.62a6.9 6.9 0 0 1-2.876-.62a6 6 0 0 1-.792-.433a4 4 0 0 1-.309-.221a.76.76 0 0 1-.21-.88L3.93 7.5H2.353a.75.75 0 0 1 0-1.5h4.102q.076 0 .141-.043l1.695-1.154c.29-.198.634-.303.985-.303h1.974V2.75a.75.75 0 0 1 1.5 0M2.193 15.198a5.4 5.4 0 0 0 2.557.635a5.4 5.4 0 0 0 2.557-.635L4.75 9.368Zm14.51-.024q.123.06.275.126c.53.223 1.305.45 2.272.45a5.85 5.85 0 0 0 2.547-.576L19.25 9.367Z" />
                        </svg>
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
                </div> -->







            </div>
        </div>
    </section>
    <FooTer />
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
import FooTer from '@/components/layout/FooTer.vue';
import NavBar from '@/components/layout/NavBar.vue';
import VisionSectionView from '@/components/sections/VisionSectionView.vue';
</script>
