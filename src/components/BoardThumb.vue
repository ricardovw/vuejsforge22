<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps({
  item: {
    type: Object,
    required: true,
  }
})
</script>

<template>
  <div class="flex flex-col">
    <img :src="item.img" class="w-24 h-24" />
    <h6>{{ item.title }}</h6>
  </div>
</template>