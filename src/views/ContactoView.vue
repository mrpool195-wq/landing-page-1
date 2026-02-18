<script setup lang="ts">
import FooTer from '@/components/layout/FooTer.vue';
import NavBar from '@/components/layout/NavBar.vue';

</script>

<template>
    <NavBar />
    <div class="backround-hero pt-[100px] pb-[100px]">
        <div class="contenedor hero">
            <div class="grid place-items-center">
                <h1 class=" text-white h1-hero">Contacto</h1>
            </div>
        </div>
    </div>
    <section class="section">
        <div class="contenedor-contactanos contenedor">
            <!-- <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d575.2138318406996!2d-89.6041710054509!3d21.003149889578932!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8f5676cbd2f6ee5d%3A0x865fd95891c1541a!2sC.%2020%20178%2C%20Jardines%20del%20Nte%2C%2097137%20M%C3%A9rida%2C%20Yuc.!5e0!3m2!1ses!2smx!4v1771441125813!5m2!1ses!2smx"
                width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"
                referrerpolicy="no-referrer-when-downgrade"></iframe> -->
            <h2 class="!text-[40px] font-bold">Envianos tus opiones</h2>
            <p class="!text[16px] text-gray-500 font-bold py-4">Recibimos feedback</p>
            <form action="">
                <div class="flex gap-4">
                    <input id="price" type="text" name="Nombre" placeholder="Nombre"
                        class="border border-gray-300 p-4 w-1/2" />
                    <input id="price" type="text" name="Correo" placeholder="Correo Electronico"
                        class="border border-gray-300 p-4 w-1/2" />
                </div>
                <br>
                <input id="price" type="text" name="Motivo" placeholder="Motivo"
                    class="border border-gray-300 p-4 w-full" />
                <br>
                <br>
                <textarea name="mensaje" id="" class="border border-gray-300 p-4 w-full resize-none"
                    placeholder="Mensaje"></textarea>
                <br><br>

                <button class="bg-(--color-acento) p-4 text-(--texto) w-64 cursor-pointer">Enviar</button>
            </form>
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