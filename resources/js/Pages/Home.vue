<script setup>
import {Head} from '@inertiajs/vue3';
import GroupList from "@/Components/GroupList.vue";
import CreatePost from "@/Components/CreatePost.vue";
import PostList from "@/Components/PostList.vue";
import FollowingList from "@/Components/FollowingList.vue";

defineProps({});

</script>

<template>
    <Head title="Social Media Website"/>
    <div class="grid lg:grid-cols-12 gap-3 p-4 h-full">
        <div class="lg:col-span-3 lg:order-1 h-full overflow-hidden">
            <GroupList/>
        </div>
        <div class="lg:col-span-3 lg:order-3 h-full overflow-hidden">
            <FollowingList/>
        </div>
        <div class="lg:col-span-6 lg:order-2 h-full overflow-hidden flex flex-col">
            <CreatePost/>
            <PostList class="flex-1"/>
        </div>

    </div>
</template>

<style>

</style>
