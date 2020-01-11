<template>
<div id="">
  <h2>Flog</h2>
  <div class="stock">
    <h3> {{ lang == 'ja' ? msg_ja : msg_en }} </h3>
    <div v-if="stock ==0">在庫なし</div>
    <div v-else>
      <ul>
      <!-- ToDo Key -->
        <li v-for="item in list" :key="item.id">{{ item.name }} x ~{{ stock }} | \ {{ item.price}}</li>
      </ul>
      <!-- ToDo 合計 -->
      <p>合計：{{ list.price }} </p>
    </div>
  </div>
</div>
</template>
<script>
export default {
  name: "",
  data: () => ({
    lang: 'ja',
    msg_ja: 'こんちくわ',
    msg_en: 'Hello',
    stock: 2,
    list:[
      {name: "itemA", price: 200},
      {name: "itemB", price: 500},
      {name: "itemC", price: 720},
    ]
  })
}
</script>
<style lang="css" scoped>
</style>

