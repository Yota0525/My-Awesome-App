<template>
  <div>
    <img
      :src="`/image/${image}`"
      alt="products"
      class="products-image"
      :style="{
        width: 'auto',
        height: 'auto',
        objectFit: 'cover',
        borderRadius: 'auto',
        marginRight: 'auto',
      }"
    />
    <div
      class="products-info"
      :style="{ display: 'flex', flexDirection: 'column' }"
    >
      <span
        class="products-name"
        :style="{ fontSize: '55px', fontWeight: 'bold' }"
        >{{ name }}</span
      >
      <span
        class="products-details"
        :style="{ fontSize: '35px', color: '#888' }"
        >{{ details }}</span
      >
    </div>
  </div>
</template>

<script setup lang="ts">
const props = defineProps({
  name: {
    type: String,
    required: true,
  },
  details: {
    type: String,
    reqired: true,
  },
  image: {
    type: String,
    required: true,
  },
});
</script>
