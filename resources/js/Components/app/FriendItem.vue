<script setup>
defineProps({
    image: String,
    title: String,
})
</script>

<template>
    <div class="mb-3 cursor-pointer hover:bg-gray-100">
        <div class="flex items-center gap-2 py-2 px-2">
            <img :src="image" alt="" class="w-[32px] rounded-full" />
            <div>
                <h3 class="text-gray-800">{{ title }}</h3>
                <div class="text-xs text-gray-400">
                    {{ description }}
                </div>
            </div>
        </div>
    </div>
</template>
