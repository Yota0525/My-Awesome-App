<template>
  <div>
    <navbar /> <!-- ナビゲーションバー -->
    <div>
      <router-view /> <!-- ページコンテンツがここに表示されます -->
    </div>
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue';

export default {
  components: {
    Navbar
  }
}
</script>

<style scoped>
/* レイアウトに適用するスタイルがあればここに記述 */
</style>