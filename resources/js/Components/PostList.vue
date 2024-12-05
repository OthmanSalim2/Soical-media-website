<script setup>

import PostItem from "@/Components/PostItem.vue";

const post1 = {
    user: {
        id: 1,
        avatar: "https://randomuser.me/api/portraits/men/34.jpg",
        name: "Othman Salim"
    },
    group: null,
    attachments: [
        {
            id: 1,
            name: "test.png",
            url: "https://picsum.photos/1000",
            mime: "image/png"
        },
        {
            id: 2,
            name: "test2.png",
            url: "https://picsum.photos/1000",
            mime: "image/png",
        },
        {
            id: 3,
            name: "Document.docx",
            url: "#",
            mime: "application/msword",
        }
    ],
    body:
        `
        <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
             when an unknown printer took a galley of type and scrambled it to make a type specimen book.
        </p>
        <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
             when an unknown printer took a galley of type and scrambled it to make a type specimen book.
        </p>
        `,
    created_at: "2024-12-2 15:12",
}

const post2 = {
    user: {
        id: 1,
        avatar: "https://randomuser.me/api/portraits/men/34.jpg",
        name: "Othman Salim"
    },
    group: {
        id: 1,
        name: "Laravel Developers"
    },
    body:
        `
        <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
             when an unknown printer took a galley of type and scrambled it to make a type specimen book.
        </p>
        <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
             when an unknown printer took a galley of type and scrambled it to make a type specimen book.
        </p>
        `,
    created_at: "2024-12-2 15:12"

}

</script>

<template>
    <div class="overflow-auto">
        <PostItem :post="post1"/>
        <PostItem :post="post2"/>
    </div>
</template>

<style scoped>

</style>
