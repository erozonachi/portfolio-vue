<template>
  <StartScreen :startChatSession="startChatSession" />
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
    }
  }
}
</script>

<style>
</style>
