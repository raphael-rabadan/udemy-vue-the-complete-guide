<template>
  <div>
    <p>Counter is: {{ doubleCounter }}</p>
    <p>Number of Clicks: {{ stringCounter }}</p>
    {{ teste }}
  </div>
</template>

<script>
import { mapGetters } from 'vuex'
import * as types from './../store/types'

export default {
  computed: {
    ...mapGetters({
      doubleCounter: types.DOUBLE_COUNTER,
      stringCounter: types.CLICK_COUNTER,
    }),
    teste() {
      return 'teste'
    },
  },
}
</script>
