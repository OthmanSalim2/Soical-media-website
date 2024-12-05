<script setup>

import TextInput from "@/Components/TextInput.vue";
import FollowerItem from "@/Components/FollowerItem.vue";
import {ref} from "vue";

const searchKeyword = ref('')
</script>

<template>
    <TextInput :model-value="searchKeyword" placeholder="Type to search" class="w-full mt-4"/>
    <div class="mt-3 h-[200px] flex-1 overflow-auto">
        <div v-if="false" class="text-gray-400 text-center p-3">
            You don't have friends yet.
        </div>
        <div v-else>
            <FollowerItem title="Mohammed Ali"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Mohammed Ali"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Mohammed Ali"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Mohammed Ali"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Mohammed Ali"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Mohammed Ali"
                          image="https://picsum.photos/200/200/?blur=2"/>
            <FollowerItem title="Elun Mask"
                          image="https://picsum.photos/200/200/?blur=2"/>
        </div>
    </div>
</template>

<style scoped>

</style>
