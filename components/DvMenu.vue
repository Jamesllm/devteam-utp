<template>
    <nav :class="{ 'bg-gray-600/25 backdrop-blur-sm': isScrolled }"
        class="py-6 bg-transparent flex justify-center items-center gap-[20em] sticky top-0 w-full text-white z-10">
        <NuxtLink to="/">
            <h2 class="text-2xl font-bold">DevTeam UTP</h2>
        </NuxtLink>
        <div class="flex gap-6">
            <div v-for="link in links" class="text-lg">
                <NuxtLink :to="link.to">{{ link.name }}</NuxtLink>
            </div>
        </div>
    </nav>
</template>
  
<script setup>
const links = [
    {
        name: 'Patrocinadores',
        to: '/patrocinadores'
    },
    {
        name: 'Acerca del evento',
        to: '/acerca-del-evento'
    },
    {
        name: 'Contacto',
        to: '/contacto'
    }
]

const isScrolled = ref(false);
const handleScroll = () => {
    isScrolled.value = window.scrollY > 0;
};

onMounted(() => {
    window.addEventListener('scroll', handleScroll);
});

onUnmounted(() => {
    window.removeEventListener('scroll', handleScroll);
});
</script>