<script setup>
import { Head, Link } from "@inertiajs/vue3";
import GroupList from "@/Components/app/GroupList.vue";
import FollowerList from "@/Components/app/FollowerList.vue";
import CreatePost from "@/Components/app/CreatePost.vue";
import PostList from "@/Components/app/PostList.vue";


defineProps({
    // canLogin: {
    //     type: Boolean,
    // },
    // canRegister: {
    //     type: Boolean,
    // },
    // laravelVersion: {
    //     type: String,
    //     required: true,
    // },
    // phpVersion: {
    //     type: String,
    //     required: true,
    // },
});
</script>

<template>
    <Head title="Aplikasi Sosmed" />
    
    <div class="grid grid-cols-12 gap-3">
        <div class="col-span-3 py-6">
            <GroupList/>
        </div>
        <div class="col-span-6">
            <CreatePost/>
            <PostList/>
        </div>
        <div class="col-span-3 py-6"><FollowerList/></div>
    </div>
</template>
