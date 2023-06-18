<script lang="ts" setup>
import { ref } from "vue";
import ListTransition from "@/components/ListTransition.vue";

const showMenu = ref(false);
</script>

<template>
  <button @click="showMenu = !showMenu">
    {{ showMenu ? "Hide" : "Show" }}
    Menu
  </button>

  <ListTransition>
    <ul v-if="showMenu">
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
    </ul>
  </ListTransition>
</template>
