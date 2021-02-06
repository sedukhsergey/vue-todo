<template>
  <div id="d">
    {{isActive}}
    <div id="event-handling">
      <p>{{ message }}</p>
      <button v-on:click="reverseMessage">Reverse Message</button>
      <Counter />
      <Conditions />
      <Loop />
    </div>
  </div>
</template>

<script>


import Counter from './Counter.vue';
import Conditions from './Conditions.vue';
import Loop from "@/components/Loop";

const HelloWorld = {
  components: {
    Counter,
    Conditions,
    Loop,
  },
  props: {
      isActive: Boolean
  },
  data() {
    return {
      message: 'Hello Vue.js!',
      count: 0,
    }
  },
  methods: {
    reverseMessage() {
      this.message = this.message
          .split('')
          .reverse()
          .join('')
    }
  }
}



export default HelloWorld
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
