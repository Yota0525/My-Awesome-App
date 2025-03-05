<template>
  <div class="products-page" :style="{ backgroundColor: '#1f75fe', color: 'white', textAlign: 'center', padding: '50px' }">
    <h1>products Introductions</h1>
    <ul class="products-list" :style="{ listStyle: 'none', padding: '0' }">
      <ProductComponent v-for="(product, index) in products" :key="index" :name="product.name" :details="product.details"
        :image="product.image" />
    </ul>
  </div>
</template>

<script setup lang="ts">
const { products } = useProducts()
</script>