<template>
  <StartScreen v-bind:startChatSession="startChatSession" />
</template>

<script>
import StartScreen from '~/components/StartScreen.vue'

export default {
  components: {
    StartScreen
  },
  data: () => ({
    username: ''
  }),
  methods: {
    startChatSession: function(username) {
      this.username = username
      console.log('username: ', this.username)
    }
  }
}
</script>

<style>
</style>
