<template>
  <div>
<!--    <button v-on:click="increment">Increment Counter</button>-->
<!--    <button v-on:click="decrement">Decrement Counter</button>-->
    {{counter}}
    <SecondCounter msg="sda"/>
  </div>
</template>

<script>
import SecondCounter from "./Form";
export default {
  components: {
    SecondCounter,
  },
  data: () => ({
      counter: 0
    }),
  methods: {
    increment: () => {
      this.counter++
    },
    decrement() {
      this.counter--
    }
  }
}
</script>


<style scoped>

</style>
