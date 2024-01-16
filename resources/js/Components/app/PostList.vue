<script setup>
import PostItem from './PostItem.vue';
const post1 = {
    user : {
        id: 1,
        avatar: 'https://randomuser.me/api/portraits/men/23.jpg',
        name: 'Nopal',
    },
    group: null,
    body : `<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat sint cum quam excepturi animi obcaecati asperiores quas, eveniet at corporis maxime quae, cumque soluta aperiam necessitatibus nulla explicabo perferendis consequuntur? </p> 
    
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat sint cum quam excepturi animi obcaecati asperiores quas, eveniet at corporis maxime quae, cumque soluta aperiam necessitatibus nulla explicabo perferendis consequuntur? </p>`,
    created_at : '2022-01-01 00:00:00',
}
</script>

<template>
    <div>
        <PostItem :post="post1"/>
    </div>
    <p></p>
</template>
