<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <part/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import part from './components/part.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    part,
}
}
</script>

