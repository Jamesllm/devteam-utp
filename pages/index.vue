<template>
  <div>
    <main>
      <hero-main />
      <section class="mb-32 max-w-screen-xl w-3/4 mx-auto">
        <div class="text-center">
          <h2 class="text-3xl sm:text-4xl font-bold text-blue-500">
            Proyectos
          </h2>
          <p class="mt-4 text-gray-300 font-semibold">
            Proyectos desarrollados por los integrantes de la DEVTEAM
          </p>
        </div>

        <div class="grid grid-cols-1 gap-4 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 lg:gap-4 mt-8">
          <div v-for="proyect in proyects">
            <Card :key="proyect" :title="proyect.title" :description="proyect.description" />
          </div>
        </div>
      </section>
      <section>
        descargar files
        <div v-for="file in files">
          <a :href="file.url">{{ file.title }}</a>
        </div>
      </section>
    </main>
  </div>
</template>

<script setup>
import pdf from "@/assets/DRAGO.pdf";
import txt from "@/assets/DRAGO.txt";

const proyects = [
  {
    title: "Barber Can",
    description: "Consiste en crear una interfaz donde el usuario permita ingresar los datos detallados de su mascota y se genere su carnet."
  },
  {
    title: "Facility Finder UTP",
    description: "Consiste en la elaboracion de una web dinámica que permita mostrar en qué ambiente le toca su clase a cualquier estudiante o docente."
  },
  {
    title: "Grades UTP",
    description: " Consiste en crear un programa que permita mostrar el récord de notas según el alumno ingresado buscándolas en un archivo CSV."
  },
  {
    title: " Plugin Minecraft",
    description: "Consiste en crear un plugin para minecraft, se usará un servidor spigot o papermc para ejecutarlo."
  },
  {
    title: "Portable Link",
    description: "Consite en la elaboracion de una web estática para poder compartir diverso link de cualquier tema o información."
  },
  {
    title: "Proyect Markdown Web",
    description: "Consiste en la elaboracion de una pagina web sobre la DevTeam - UTP."
  },
  {
    title: "Random Generator",
    description: "Consiste en elaborar una web dinámica que permita generar datos de cualquier tipo."
  },
  {
    title: "Text Encrypt",
    description: "Consiste en elaborar una web que permita encriptar texto y desencriptarlo."
  }
]

const files = [
  {
    title: "PDF",
    url: pdf
  },
  {
    title: "TXT",
    url: txt
  }
]
</script>