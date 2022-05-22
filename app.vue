<template>
  <div>
    <NuxtWelcome />
    <Dialog :open="isOpen" @close="toggleModal"> </Dialog>
  </div>
</template>

<script setup lang="ts">
import { Dialog } from "@headlessui/vue";

const isOpen = ref(false);

const toggleModal = () => {
  isOpen.value = isOpen.value ? false : true;
};
</script>

