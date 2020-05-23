<template>
  <div>
    <h1>{{ msg }}</h1>
    <h3>Count: {{ count }}</h3>
    <button @click="increase">click me!</button>
  </div>
</template>
<script lang="ts">
import { defineComponent,ref } from 'vue'
export default defineComponent({
  props: {
    msg: {
      type: String,
      default: 'welcome to study vue3！'
    }
  },
  setup(){
    const count = ref(0)
    const increase = () => {
      count.value++
    }

    return {
      count,
      increase
    }
  }
})
</script>