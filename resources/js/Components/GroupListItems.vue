<script setup>

import TextInput from "@/Components/TextInput.vue";
import GroupItem from "@/Components/GroupItem.vue";
import {ref} from "vue";

const searchKeyword = ref('')
</script>

<template>
    <TextInput :model-value="searchKeyword" placeholder="Type to search" class="w-full mt-4"/>
    <div class="mt-3 h-[200px] flex-1 overflow-auto">
        <div v-if="false" class="text-gray-400 text-center p-3">
            You are not joined to any groups.
        </div>
        <div v-else>
            <GroupItem title="Laravel Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
            <GroupItem title="Vue.js Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
            <GroupItem title="Vue.js Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
            <GroupItem title="Vue.js Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
            <GroupItem title="Vue.js Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
            <GroupItem title="Vue.js Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
            <GroupItem title="Vue.js Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
            <GroupItem title="Laravel Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
            <GroupItem title="Vue.js Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
            <GroupItem title="Laravel Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
            <GroupItem title="Vue.js Developers"
                       description="Lorem Ipsum is simply dummy text of the printing industry."
                       image="https://picsum.photos/200/200/?blur=2"/>
        </div>
    </div>
</template>

<style scoped>

</style>
