<template>
    <article
        class="relative flex flex-col bg-gray-600/10 shadow-md border-[1px] border-gray-700 rounded-xl w-full h-full hover:border-blue-500 transition-all duration-300">
        <div class="p-6">
            <h5 class="mb-2 text-xl font-semibold">
                {{ title }}
            </h5>
            <p class="text-gray-200 text-sm">
                {{ description }}
            </p>
        </div>
    </article>
</template>

<script setup>
const props = defineProps({
    title: {
        type: String,
        required: true,
    },
    description: {
        type: String,
        required: true,
    }
});
</script>
