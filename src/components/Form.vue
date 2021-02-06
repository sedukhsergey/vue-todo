<template>
  <div id="two-way-binding">
    <input v-model="message" />
    <input v-model="email" type="email" />
    <input v-model="password" type="password" />
  </div>
</template>

<script>

  export default {
    data() {
      return {
        message: '',
        email: '',
        password: ''
      }
    },
  }
</script>
