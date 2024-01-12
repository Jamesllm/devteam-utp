<template>
    <div
        class="mt-[-80px] bg-gray-950 bg-[radial-gradient(ellipse_80%_80%_at_50%_-20%,rgba(120,119,198,0.3),rgba(255,255,255,0))]">
        <section class="mx-auto max-w-screen-xl w-3/4 px-4 py-32 lg:flex lg:h-screen lg:items-center">
            <div class="grid grid-cols-1 gap-4 sm:grid-cols-2 lg:gap-8">
                <div>
                    <NuxtLink to="/acerca-del-evento">
                        <dv-badge />
                    </NuxtLink>
                    <h1
                        class="bg-gradient-to-r from-green-300 via-blue-500 to-purple-600 bg-clip-text text-3xl font-extrabold text-transparent sm:text-6xl">
                        DevTeam UTP
                    </h1>
                    <p class="mt-4 text-lg text-gray-300">
                        La DEVTEAM es una competencia en la que se plantean diversos
                        proyectos en los cuales cualquier estudiante de la universidad de la
                        carrera de Ingieneria de Sistemas puede acceder, puede elegir a que
                        grupo pertenecer e incluso pertenecer a varios.
                    </p>

                    <div class="flex gap-4 mt-8">
                        <button
                            class="inline-block rounded-lg bg-blue-600 px-5 py-3 text-sm font-medium text-white transition-colors duration-300 hover:bg-blue-500">
                            Conocer más
                        </button>
                        <button
                            class="inline-block rounded-lg bg-gray-800 px-5 py-3 text-sm font-medium text-white transition-colors duration-300 hover:bg-gray-700">
                            Ver proyectos ⭐
                        </button>
                    </div>
                </div>
                <div>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Exercitationem tempora facilis expedita.
                    Quae ratione veniam in, aliquid culpa aspernatur ullam optio nemo deleniti, voluptatibus,
                    consectetur aut omnis natus sapiente ipsam.</div>
            </div>
        </section>
    </div>
</template>

<script>
</script>