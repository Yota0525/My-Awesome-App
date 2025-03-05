<template>
  <div class="singers-page" :style="{ backgroundColor: '#1f75fe', color: 'white', textAlign: 'center', padding: '50px' }">
    <h1>singers Introductions</h1>
    <ul class="singers-list" :style="{ listStyle: 'none', padding: '0' }">
      <SingerComponent v-for="(singer, index) in singers" :key="index" :name="singer.name" :details="singer.details"
        :image="singer.image" />
    </ul>
  </div>
</template>

<script setup lang="ts">
const { singers } = useSingers()
</script>