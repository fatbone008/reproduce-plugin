<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <lib-testing></lib-testing>
    <my-testing></my-testing>
  </div>
</template>

<script>
import LibTesting from 'lib';
import MyTesting from "@/components/MyTesting";
import {provide} from 'vue';
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  setup() {
    provide('pass', "I'm provider value")
  },
  components: {
    LibTesting,
    MyTesting
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
