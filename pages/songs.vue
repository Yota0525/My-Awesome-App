<template>
  <div class="songs-page" :style="{ backgroundColor: '#1f75fe', color: 'white', textAlign: 'center', padding: '50px' }">
    <h1>songs Introductions</h1>
    <ul class="songs-list" :style="{ listStyle: 'none', padding: '0' }">
      <SongComponent v-for="(song, index) in songs" :key="index" :name="song.name" :details="song.details"
        :image="song.image" />
    </ul>
  </div>
</template>

<script setup lang="ts">
const { songs } = useSongs()
</script>
