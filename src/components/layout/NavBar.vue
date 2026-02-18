<template>
    <nav class="backround-nav">
        <div class="contenedor flex justify-between items-center p-4">
            <!-- Logo -->
            <div class="logo">
                <a href="">
                    <!-- <h1 class="text-blue-100">Tecnologias</h1> -->
                    <img src="/src/assets/img/TECNOLOGIAS INTEGRALES - white version.png" class="w-70" alt="">
                </a>
            </div>

            <!-- Menú principal (desktop) -->
            <div class="opciones">
                <ul class="menu-list">
                    <a href="">
                        <router-link to="/">Inicio</router-link>
                    </a>
                    <a href="">
                        <router-link to="/quienes-somos">Quienes somos</router-link>
                    </a>
                    <a href="">
                        <router-link to="/contacto">Contacto</router-link>
                    </a>
                </ul>
            </div>

            <!-- Contacto (desktop) -->
            <div class="contacto text-blue-200">
                Contacto &nbsp; 9997675868
            </div>

            <!-- Botón hamburguesa (móvil) -->
            <button class="menu-toggle" @click="menuAbierto = !menuAbierto" aria-label="Abrir menú">
                <iconMenu />
            </button>
        </div>

        <!-- Menú móvil desplegable -->
        <!-- <div v-if="menuAbierto" class="mobile-menu">
            <ul class="mobile-menu-list">
                <router-link to="/" @click="menuAbierto = false">Inicio</router-link>
                <router-link to="/quienes-somos" @click="menuAbierto = false">Quienes somos</router-link>
                <a href="" @click="menuAbierto = false">
                    <li>Contáctanos</li>
                </a>

                <li class="mobile-contacto">
                    <a href="">Contactanos</a>
                </li>
            </ul>
        </div> -->
        <Transition name="sandwich">
            <div v-if="menuAbierto" class="mobile-menu">
                <ul class="mobile-menu-list">
                    <router-link to="/" @click="menuAbierto = false">Inicio</router-link>
                    <router-link to="/quienes-somos" @click="menuAbierto = false">Quienes somos</router-link>
                    <router-link to="/contacto" @click="menuAbierto = false">Contacto</router-link>
                </ul>
            </div>
        </Transition>

    </nav>
</template>

<script setup>
import iconMenu from '@/components/icons/iconMenu.vue';

import { ref } from 'vue'

const menuAbierto = ref(false)
</script>

<style scoped>
.sandwich-enter-active,
.sandwich-leave-active {
    transition: max-height 0.28s ease, opacity 0.28s ease, transform 0.28s ease;
    overflow: hidden;
}

.sandwich-enter-from,
.sandwich-leave-to {
    max-height: 0;
    opacity: 0;
    transform: translateY(-8px);
}

.sandwich-enter-to,
.sandwich-leave-from {
    max-height: 320px;
    opacity: 1;
    transform: translateY(0);
}

.backround-nav {
    background-color: var(--color-pricipal);
}

.logo h1 {
    font-weight: bold;
    font-size: 1.5rem;
    margin: 0;
}

.opciones,
.contacto {
    display: flex;
    align-items: center;
}

.menu-list {
    list-style: none;
    display: flex;
    gap: 1.5rem;
    margin: 0;
    padding: 0;
}

.menu-list a {
    text-decoration: none;
    color: #e0e0e0;
    font-weight: 500;
    transition: color 0.3s ease;
}

.menu-list a:hover {
    color: #64b5f6;
}

.menu-list li {
    margin: 0;
}

.contacto {
    cursor: pointer;
    padding: 0.5rem 1rem;
    border-radius: 0.5rem;
    transition: background-color 0.3s ease;
}

.contacto:hover {
    background-color: rgba(100, 181, 246, 0.1);
}

.menu-toggle {
    display: none;
    background: none;
    border: none;
    cursor: pointer;
    padding: 0;
    margin: 0;
}

.menu-icon {
    width: 2.5rem;
    height: auto;
    filter: brightness(0.9);
    transition: filter 0.3s ease;
}

.menu-toggle:hover .menu-icon {
    filter: brightness(1.2);
}

/* Menú móvil (inicialmente oculto) */
.mobile-menu {
    display: none;
}

.mobile-menu-list {
    list-style: none;
    margin: 0;
    padding: 1rem 0;
}

.mobile-menu-list a {
    display: block;
    padding: 1rem 1.5rem;
    color: #e0e0e0;
    text-decoration: none;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    transition: background-color 0.3s ease;
}

.mobile-menu-list a:hover {
    background-color: rgba(100, 181, 246, 0.1);
    color: #64b5f6;
}

.mobile-menu-list li {
    margin: 0;
}

.mobile-contacto {
    background-color: rgba(100, 181, 246, 0.1);
    border-top: 2px solid #64b5f6;
}

.mobile-contacto a {
    border: none;
    color: #64b5f6;
    font-weight: 600;
}

/* MEDIA QUERIES - Punto de quiebre: 768px (tablet/mobile) */
@media (max-width: 768px) {

    /* Ocultar menú de escritorio */
    .opciones {
        display: none;
    }

    .contacto {
        display: none;
    }

    /* Mostrar botón hamburguesa */
    .menu-toggle {
        display: block;
    }

    /* Mostrar menú móvil cuando esté abierto */
    .mobile-menu {
        display: block;
        background-color: rgba(0, 0, 0, 0.05);
        border-top: 1px solid rgba(255, 255, 255, 0.1);
    }

    /* Ajustar padding del contenedor */
    .contenedor {
        padding-left: 1rem;
        padding-right: 1rem;
    }
}

/* MEDIA QUERIES - Puntos de quiebre adicionales */
/* @media (max-width: 600px) {
    .logo h1 {
        font-size: 1.25rem;
    }

    .menu-icon {
        width: 2rem;
    }

    .mobile-menu-list a {
        padding: 0.875rem 1rem;
    }
}

@media (max-width: 480px) {
    .logo h1 {
        font-size: 1rem;
    }

    .menu-icon {
        width: 1.75rem;
    }
} */
</style>
