<template>
  <div class="home">
    <Counter msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import Counter from '@/components/Counter'

export default {
  name: 'Home',
  components: {
    Counter
  }
}
</script>
