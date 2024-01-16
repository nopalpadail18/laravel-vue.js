<script setup>
import { ref } from "vue";
const PostCreating = ref(false);
</script>

<template>
    <div class="py-6">
        <div
            @click="PostCreating = true"
            class="py-3 px-2 text-gray-500 border border-gray-300 rounded mb-3"
        >
            Klik Disini Untuk Mebuat Postingan Baru
        </div>
        <div v-if="PostCreating" class="flex gap-2 justify-between">
            <button
                type="submit"
                class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 relative"
            >
                Lampirkan File
                <input
                    type="file"
                    class="absolute left-0 right-0 top-0 bottom-0 opacity-0"
                />
            </button>
            <button
                type="submit"
                class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600" 
            >
                Kirim
            </button>
        </div>
    </div>
</template>
