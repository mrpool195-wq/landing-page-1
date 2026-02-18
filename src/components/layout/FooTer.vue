<template>
    <footer class="section bg-(--color-pricipal)">
        <div class="contenedor contenedor-footer flex flex-wrap gap-8">
            <div class="flex-1 min-w-[280px] px-6">
                <div>
                    <a href=""><router-link to="/"><img src="/src/assets/img/TECNOLOGIAS INTEGRALES - white version.png"
                                class="w-80" alt=""></router-link></a>

                </div>
                <p class="text-white py-[40px]">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ut eveniet
                    omnis
                    velit
                    numquam dolore optio
                    cum non sed nesciunt nihil ab blanditiis odit excepturi eaque, voluptas officia quod quibusdam
                    libero.</p>

                <div class="flex gap-4 py-2">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                        <g fill="none" stroke="white" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
                            <path d="M3 7a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z" />
                            <path d="m3 7l9 6l9-6" />
                        </g>
                    </svg>
                    <p class="text-white pb-4">example.email@test.test</p>
                </div>

                <div class="flex gap-4 py-2">
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 14 14">
                        <path fill="none" stroke="white" stroke-linecap="round" stroke-linejoin="round"
                            d="M8.76 13a3.19 3.19 0 0 0 4-.44l.45-.44a1.08 1.08 0 0 0 0-1.51L11.3 8.72a1.07 1.07 0 0 0-1.5 0h0a1.08 1.08 0 0 1-1.51 0l-3-3a1.06 1.06 0 0 1 0-1.51h0a1.07 1.07 0 0 0 0-1.5L3.39.81a1.08 1.08 0 0 0-1.51 0l-.44.45a3.19 3.19 0 0 0-.44 4A28.94 28.94 0 0 0 8.76 13Z" />
                    </svg>
                    <p class="text-white pb-4">
                        +52 (999) 9997675868
                    </p>
                </div>

                <div class="flex gap-4 py-2">
                    <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24">
                        <g fill="none" stroke="white" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
                            <circle cx="12" cy="10" r="3" />
                            <path
                                d="M12 2a8 8 0 0 0-8 8c0 1.892.402 3.13 1.5 4.5L12 22l6.5-7.5c1.098-1.37 1.5-2.608 1.5-4.5a8 8 0 0 0-8-8" />
                        </g>
                    </svg>
                    <p class="text-white pb-4">

                        CALLE 20 EXT. 178 ENTRE CALLE 15 Y 17 COLONIA MEXICO ORIENTE, MERIDA,
                        YUCATAN,
                        C.P. 97137
                    </p>
                </div>
            </div>

            <div class="flex-1 min-w-[280px] flex justify-around px-6">
                <div>
                    <h2 class="text-white pb-4 font-bold">Servicios</h2>
                    <ul class="list-none text-white">
                        <li class="py-4"><router-link to="/">Desarrollo a medida</router-link></li>
                        <li class="py-4"><router-link to="/quienes-somos">Infraestructura Cloud</router-link></li>
                        <li class="py-4"><router-link to="/contacto">Ciberseguridad</router-link></li>
                        <li class="py-4"><router-link to="/contacto">Inteligencia Artificial</router-link></li>
                        <li class="py-4"><router-link to="/contacto">Analisis de datos</router-link></li>
                        <li class="py-4"><router-link to="/contacto">Apps Moviles</router-link></li>
                    </ul>
                </div>
                <div class="">
                    <h2 class="text-white pb-4 font-bold">Empresa</h2>
                    <ul class="list-none text-white">
                        <li class="py-4"><router-link to="/">Inicio</router-link></li>
                        <li class="py-4"><router-link to="/quienes-somos">Quienes somos</router-link></li>
                        <li class="py-4"><router-link to="/contacto">Contacto</router-link></li>
                    </ul>
                </div>
            </div>

            <div class="flex-1 min-w-[280px] px-6">
                <h2 class="text-white pb-4 font-bold">Social</h2>
                <h2 class="text-white pb-4 font-bold">Nuestras Redes</h2>
                <ul class="list-none flex gap-4">
                    <li>
                        <a href="" class="inline-block bg-(--texto) p-[5px] rounded-md">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                                <g fill="none">
                                    <path stroke="currentColor"
                                        d="M3 11c0-3.771 0-5.657 1.172-6.828S7.229 3 11 3h2c3.771 0 5.657 0 6.828 1.172S21 7.229 21 11v2c0 3.771 0 5.657-1.172 6.828S16.771 21 13 21h-2c-3.771 0-5.657 0-6.828-1.172S3 16.771 3 13z" />
                                    <circle cx="16.5" cy="7.5" r="1.5" fill="currentColor" />
                                    <circle cx="12" cy="12" r="3.5" stroke="currentColor" />
                                </g>
                            </svg>
                        </a>
                    </li>
                    <li>
                        <a href="" class="inline-block bg-(--texto) p-[5px] rounded-md">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 512 512">
                                <path
                                    d="M288 192v-38.1c0-17.2 3.8-25.9 30.5-25.9H352V64h-55.9c-68.5 0-91.1 31.4-91.1 85.3V192h-45v64h45v192h83V256h56.4l7.6-64h-64z"
                                    fill="currentColor" />
                            </svg>
                        </a>
                    </li>
                    <li>
                        <a href="" class="inline-block bg-(--texto) p-[5px] rounded-md">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                                <path fill="currentColor" fill-rule="evenodd"
                                    d="M12 2.928a9.072 9.072 0 0 0-7.646 13.956l-1.542 3.568a.75.75 0 0 0 .897 1.018l4.395-1.275A9.072 9.072 0 1 0 12 2.928m1.372 11.825c-.372.22-1.187.287-2.736-1.262s-1.482-2.363-1.262-2.736c.56-.057 1.097-.432 1.595-.93c.369-.369.07-1.264-.666-2c-.737-.737-1.632-1.035-2-.667c-2.372 2.371-1.184 5.482 1 7.667c2.214 2.214 5.238 3.428 7.667 1c.368-.369.07-1.264-.667-2c-.737-.737-1.632-1.035-2-.667c-.499.498-.874 1.035-.93 1.595"
                                    clip-rule="evenodd" />
                            </svg>
                        </a>
                    </li>
                    <li>
                        <a href="" class="inline-block bg-(--texto) p-[5px] rounded-md">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 20 20">
                                <path fill="currentColor"
                                    d="M5 3c0 1.062-.71 1.976-2.001 1.976C1.784 4.976 1 4.114 1 3.052C1 1.962 1.76 1 3 1s1.976.91 2 2M1 19V6h4v13zm6-8.556c0-1.545-.051-2.836-.102-3.951h3.594l.178 1.723h.076c.506-.811 1.746-2 3.822-2C17.1 6.216 19 7.911 19 11.558V19h-4v-6.861c0-1.594-.607-2.81-2-2.81c-1.062 0-1.594.86-1.873 1.569c-.102.254-.127.608-.127.963V19H7z" />
                            </svg>

                        </a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="contenedor pt-[50px]">
            <hr class="bg-(--texto) text-(--texto)">

        </div>
    </footer>
</template>
<script setup>
</script>