<template>
    <footer class="bg-gray-600/10 text-center py-6">
        &copy;{{ getYear }} DevTeam UTP. Todos los derechos reservados.
    </footer>
</template>

<script setup>
const today = new Date();
const getYear = today.getFullYear();
</script>