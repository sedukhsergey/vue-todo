<template>
  <div>
    <span v-if="seen">Now you see me</span>
    <button v-on:click="handleSwitchSeen">Switch</button>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        seen: true
      }
    },
    methods: {
      handleSwitchSeen() {
        this.seen = !this.seen;
      }
    }
  }
</script>
