<template>
  <div>
    <NuxtWelcome />
  </div>
  <Dialog :open="isOpen" @close="toggleModal"> </Dialog>
</template>

<script setup lang="ts">
import { Dialog } from "@headlessui/vue";

const isOpen = ref(false);

const toggleModal = () => {
  isOpen.value = isOpen.value ? false : true;
};
</script>

