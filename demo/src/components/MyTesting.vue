<template>
  <div class="love">
    <span>click me</span>
    <button>I'm button</button>
  </div>
</template>

<script>
import {reactive, inject} from 'vue'
export default {
  name: "MyTesting",
  setup() {
    console.log('Im in setup()');
    const obj = reactive({
      a: 1,
      b: 0
    });
    const sarah = inject('pass', "I'm default value")
    return {
      sarah,
      obj
    }
  },
  mounted() {
    console.log('Testing component mounted.');
  }
}
</script>

<style scoped>

</style>
