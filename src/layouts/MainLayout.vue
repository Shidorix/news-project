<template>
  <NewsHeader />

  <router-view v-slot="{ Component }">
    <keep-alive>
      <component :is="Component" />
    </keep-alive>
  </router-view>
</template>

<script setup lang="ts">
import NewsHeader from "../components/NewsHeader.vue";
</script>
