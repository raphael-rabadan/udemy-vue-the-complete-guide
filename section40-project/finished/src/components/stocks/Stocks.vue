<template>
  <div>
    <app-stock v-for="(stock, i) in stocks" :stock="stock" :key="i"></app-stock>
  </div>
</template>

<script>
import Stock from './Stock.vue'

export default {
  components: {
    appStock: Stock,
  },
  computed: {
    stocks() {
      return this.$store.getters.stocks
    },
  },
}
</script>
