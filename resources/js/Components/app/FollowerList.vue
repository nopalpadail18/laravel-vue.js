<script setup>
import TextInput from "@/Components/TextInput.vue";
import { ref } from "vue";
import FriendItem from "./FriendItem.vue";

const searchKeyword = ref("");
</script>

<template>
    <div class="px-3">
        <h2 class="text-2xl font-bold mb-4">Teman Saya</h2>
        <TextInput :model-value="searchKeyword" placeholder="Type to Search" />
        <div class="py-8">
            <div v-if="false" class="text-gray-400 flex text-center py-8">
                Anda Belum Mengikuti Siapa pun.
            </div>
            <div v-else>
                <FriendItem
                    image="https://picsum.photos/100"
                    title="Jhon Doe"
                />
                <FriendItem
                    image="https://picsum.photos/100"
                    title="Ellon Musk"
                />
            </div>
        </div>
    </div>
</template>
