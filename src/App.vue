<template>
  <div>{{ msg }}</div>
</template>

<script>
import { reactive, toRefs } from 'vue'
export default {
  setup() {
    const state = reactive({
      msg: 'hello vue2'
    })
    return {
      ...toRefs(state)
    }
  }
}
</script>