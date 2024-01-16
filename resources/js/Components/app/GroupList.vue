<script setup>
import GroupItem from "@/Components/app/GroupItem.vue";
import TextInput from "@/Components/TextInput.vue";
import { ref } from "vue";

const searchKeyword = ref("");
</script>

<template>
    <div class="px-3">
        <h2 class="text-2xl font-bold mb-4">Grup Saya</h2>
        <TextInput :model-value="searchKeyword" placeholder="Type to Search" />
        <div class="py-8">
            <div v-if="false" class="text-gray-400 flex text-center py-8">
                Your are not joined to any group
            </div>
            <div v-else>
                <GroupItem
                    image="https://picsum.photos/100"
                    title="Vue.js Laravel Developers"
                    description="Lorem, ipsum dolor sit amet consectetur
                                adipisicing elit. Accusantium, itaque?"
                />
                <GroupItem
                    image="https://picsum.photos/100"
                    title="Vue.js Laravel Developers"
                    description="Lorem, ipsum dolor sit amet consectetur
                                adipisicing elit. Accusantium, itaque?"
                />
            </div>
        </div>
    </div>
</template>
