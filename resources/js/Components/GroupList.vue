<script setup>

import {Disclosure, DisclosureButton, DisclosurePanel} from "@headlessui/vue";
import GroupListItems from "@/Components/GroupListItems.vue";
</script>

<template>
    <div class="px-3 bg-white border rounded shadow h-full py-3 overflow-hidden">
        <div class="block lg:hidden">
            <Disclosure v-slot="{ open }">
                <DisclosureButton class="w-full">
                    <div class="flex justify-between items-center">
                        <h2 class="text-xl font-bold">My Groups</h2>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                             stroke="currentColor" class="w-6 h-6 transition-all"
                             :class="open ? 'rotate-90 transform' : ''">
                            <path stroke-linecap="round" stroke-linejoin="round" d="m8.25 4.5 7.5 7.5-7.5 7.5"/>
                        </svg>
                    </div>
                </DisclosureButton>
                <DisclosurePanel>
                    <GroupListItems/>
                </DisclosurePanel>
            </Disclosure>
        </div>
        <div class="h-full flex-col overflow-hidden hidden lg:flex">
            <h2 class="text-xl font-bold mb-4">My Groups</h2>
            <GroupListItems/>
        </div>
    </div>
</template>

<style scoped>

</style>
