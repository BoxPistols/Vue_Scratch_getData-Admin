<template>
<div id="">
  <h2>Flog</h2>
  <div class="stock">
    <div v-if="stock ==0">在庫なし</div>
    <div v-else>{{ price}}円</div>
  </div>
</div>
</template>
<script>
export default {
  name: "",
  data: () => ({
    price: 100,
    stock: 0
  })
}
</script>
<style lang="css" scoped>
</style>

