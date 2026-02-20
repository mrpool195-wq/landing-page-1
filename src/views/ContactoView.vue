<script setup>
import FooTer from '@/components/layout/FooTer.vue';
import NavBar from '@/components/layout/NavBar.vue';
import { ref } from 'vue';

// Variables reactivas para los campos del formulario
const nombre = ref('');
const correo = ref('');
const asunto = ref('');
const mensaje = ref('');

// Función para validar el formulario
function validarForm() {
    // Verificar que ningún campo esté vacío
    if (!nombre.value.trim() || !correo.value.trim() || !asunto.value.trim() || !mensaje.value.trim()) {
        alert('Todos los campos son obligatorios.');
        return false;
    }

    // Verificar que el correo contenga '@'
    if (!correo.value.includes('@')) {
        alert('Por favor, ingresa un correo electrónico válido.');
        return false;
    }

    return true;
}

// Función para enviar el formulario
async function enviarFormulario() {
    if (!validarForm()) {
        return;
    }

    // Preparar los datos para enviar
    const datos = {
        nombre: nombre.value,
        correo: correo.value,
        asunto: asunto.value,
        mensaje: mensaje.value
    };

    try {
        // Enviar con POST a contacto.php
        const response = await fetch('/assets/contacto.php', {
            method: 'POST',
            headers: {
                'Content-Type': 'application/json'
            },
            body: JSON.stringify(datos)
        });

        if (response.ok) {
            alert('Mensaje enviado exitosamente.');
            // Limpiar el formulario
            nombre.value = '';
            correo.value = '';
            asunto.value = '';
            mensaje.value = '';
        } else {
            alert('Error al enviar el mensaje.');
        }
    } catch (error) {
        console.error('Error:', error);
        alert('Error al enviar el mensaje.');
    }
}
</script>

<template>
    <NavBar />
    <div
        class="bg-(--color-pricipal) bg-[radial-gradient(#4F4E50_1px,transparent_1px)] bg-[size:20px_20px]  pt-[100px] pb-[100px]">
        <div class="contenedor hero">
            <div class="grid place-items-center">
                <h1 class=" text-white h1-hero">Contacto</h1>
                <p class="text-(--blanco1) !text-[20px] py-6">Envianos tus comentarios o sugerencias.
                </p>
            </div>
        </div>
    </div>
    <section class="section">
        <div class="contenedor-contactanos contenedor">
            <div class="contenedor-formulario">

                <div class="flex gap-4">
                    <div class="w-1/2 p-[30px] ">

                        <h2 class="!text-[40px] font-bold">Nuestra información</h2>


                        <div class="flex gap-4 py-4">

                            <div class="p-2 bg-(--color-pricipal) rounded-xl">
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 14 14">
                                    <path fill="none" stroke="var(--color-boton1)" stroke-linecap="round"
                                        stroke-linejoin="round"
                                        d="M8.76 13a3.19 3.19 0 0 0 4-.44l.45-.44a1.08 1.08 0 0 0 0-1.51L11.3 8.72a1.07 1.07 0 0 0-1.5 0h0a1.08 1.08 0 0 1-1.51 0l-3-3a1.06 1.06 0 0 1 0-1.51h0a1.07 1.07 0 0 0 0-1.5L3.39.81a1.08 1.08 0 0 0-1.51 0l-.44.45a3.19 3.19 0 0 0-.44 4A28.94 28.94 0 0 0 8.76 13Z" />
                                </svg>
                            </div>

                            <div>
                                <h4>Télefono</h4>
                                <a href="">+52 (999) 9997675868</a>
                            </div>

                        </div>

                        <div class="flex gap-4 py-4">

                            <div class="p-2 bg-(--color-pricipal) rounded-xl h-12">
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24">
                                    <g fill="none" stroke="var(--color-boton1)" stroke-linecap="round"
                                        stroke-linejoin="round" stroke-width="2">
                                        <circle cx="12" cy="10" r="3" />
                                        <path
                                            d="M12 2a8 8 0 0 0-8 8c0 1.892.402 3.13 1.5 4.5L12 22l6.5-7.5c1.098-1.37 1.5-2.608 1.5-4.5a8 8 0 0 0-8-8" />
                                    </g>
                                </svg>
                            </div>

                            <div>
                                <h4>Dirección</h4>
                                <a href="">CALLE 20 EXT. 178 ENTRE CALLE 15 Y 17 COLONIA MEXICO ORIENTE, MERIDA,YUCATAN,
                                    C.P. 97137</a>
                            </div>

                        </div>

                        <div class="flex gap-4 py-4">

                            <div class="p-2 bg-(--color-pricipal) rounded-xl h-12">
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24">
                                    <g fill="none" stroke="var(--color-boton1)" stroke-linecap="round"
                                        stroke-linejoin="round" stroke-width="2">
                                        <path
                                            d="M3 7a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z" />
                                        <path d="m3 7l9 6l9-6" />
                                    </g>
                                </svg>
                            </div>

                            <div>
                                <h4>Correo Electronico</h4>
                                <a href="">example.email@test.test</a>
                            </div>

                        </div>


                        <!-- <div>
                            <div>
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24">
                                    <g fill="none" stroke="var(--color-boton1)" stroke-linecap="round"
                                        stroke-linejoin="round" stroke-width="2">
                                        <path
                                            d="M3 7a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z" />
                                        <path d="m3 7l9 6l9-6" />
                                    </g>
                                </svg>
                            </div>
                            <h4>Correo</h4>
                            <a href="">+52 (999) 9997675868</a>
                        </div>

                        <div>
                            <div>
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24">
                                    <g fill="none" stroke="var(--color-boton1)" stroke-linecap="round"
                                        stroke-linejoin="round" stroke-width="2">
                                        <path
                                            d="M3 7a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z" />
                                        <path d="m3 7l9 6l9-6" />
                                    </g>
                                </svg>
                            </div>
                            <h4>Dirección</h4>
                            <a href="">+52 (999) 9997675868</a>
                        </div> -->
                    </div>

                    <div class="bg-[#CCCACF] p-[50px] rounded-xl w-1/2">

                        <h2 class="!text-[40px] font-bold">Envianos tus opiones</h2>
                        <p class="!text[16px] text-gray-500 py-4">Obligatorio<span class="text-red-500">*</span></p>

                        <form @submit.prevent="enviarFormulario">

                            <div class="flex gap-4">

                                <!-- campo nombre -->
                                <div class="w-1/2">
                                    <label for="nombre" class="block text-sm font-medium pb-2">
                                        Nombre completo <span class="text-red-500">*</span>
                                    </label>
                                    <input id="nombre" type="text" name="nombre" placeholder="Nombre"
                                        class="rounded-md border border-gray-300 p-4 w-full bg-(--blanco1)"
                                        v-model="nombre" />
                                </div>

                                <!-- campo correo electronico -->

                                <div class="w-1/2">
                                    <label for="correo" class="block text-sm font-medium pb-2">
                                        Correo electronico <span class="text-red-500">*</span>
                                    </label>
                                    <input id="correo" type="email" name="correo"
                                        placeholder="tucorreo@ejemplocorreo.com"
                                        class="rounded-md border border-gray-300 p-4 w-full bg-(--blanco1)"
                                        v-model="correo" />
                                </div>

                            </div>

                            <!-- campo asunto -->

                            <div class="py-4">
                                <label for="asunto" class="block text-sm font-medium pb-2">
                                    Asunto <span class="text-red-500">*</span>
                                </label>
                                <input id="asunto" type="text" name="asunto" placeholder="Asunto"
                                    class="rounded-md border border-gray-300 p-4 w-full bg-(--blanco1)"
                                    v-model="asunto" />
                            </div>


                            <!-- campo mensaje -->

                            <div class="py-4">
                                <label for="mensaje" class="block text-sm font-medium pb-2">
                                    Mensaje <span class="text-red-500">*</span>
                                </label>
                                <textarea name="mensaje" id="mensaje"
                                    class="rounded-md border border-gray-300 p-4 w-full resize-none bg-(--blanco1)"
                                    placeholder="Escribe tu mensaje..." v-model="mensaje"></textarea>
                            </div>


                            <button type="submit"
                                class="bg-(--color-boton1) inline-block py-4 px-8 rounded-md font-semibold !text-[14px] text-(--blanco1) transition-shadow duration-300 hover:shadow-[0_0_16px_#dddddd] w-60 cursor-pointer">
                                Enviar
                            </button>

                        </form>
                    </div>
                </div>
            </div>
            <br>
            <div class="w-full  contenedor-iframe rounded-xl">
                <iframe
                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d575.2138318406996!2d-89.6041710054509!3d21.003149889578932!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8f5676cbd2f6ee5d%3A0x865fd95891c1541a!2sC.%2020%20178%2C%20Jardines%20del%20Nte%2C%2097137%20M%C3%A9rida%2C%20Yuc.!5e0!3m2!1ses!2smx!4v1771441125813!5m2!1ses!2smx"
                    width="100%" height="450" style="border:0;" loading="lazy" class="rounded-xl"
                    referrerpolicy="no-referrer-when-downgrade">
                </iframe>
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

/* .backround-hero {
    background-color: var(--color-pricipal);
} */

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