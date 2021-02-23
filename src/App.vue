<template>
  <div id="app">
    <button @click="result">結果を見る</button>
  </div>
</template>

<script>
export default {
  el: '#app',
  data() {
    return {
      list: [
        '大吉',
        '中吉',
        '小吉',
        '末吉'
      ],
    }
  },
  methods: {
    result: function() {
      const num = Math.floor(Math.random() * this.list.length)
      alert(this.list[num])
    }
  }
};
</script>


