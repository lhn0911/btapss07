<template>
  <div>
    <button @click="openForm">Add user</button>
    <FormAddUser :isOpen="isFormOpen" @close-form="closeForm" />
  </div>
</template>

<script setup>
import { ref } from "vue";
import FormAddUser from "@/components/b8/FormAddUser.vue";

const isFormOpen = ref(false);

const openForm = () => {
  isFormOpen.value = true;
};
const closeForm = () => {
  isFormOpen.value = false;
};
</script>
