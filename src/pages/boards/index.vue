<script setup lang="ts">
import { ref } from 'vue'

const thumbs = ref([
  { title: 'First', img: '../assets/images/thumb1.jpg' },
  { title: 'Second', img: '../assets/images/thumb2.jpg' },
  { title: 'Third', img: '../assets/images/thumb3.jpg' },
])
</script>

<template>
  <div class="flex space-x-5">
    <BoardThumb
      v-for="thumb in thumbs"
      :item="thumb"
    />
    <BoardThumbNew />
  </div>
</template>