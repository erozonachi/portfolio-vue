<template>
  <StartScreen v-bind:startChatSession="startChatSession" v-if="!username" />
  <div v-else>
    <AppBar />
    <Chats :username="username" />
    <FootBar />
  </div>
</template>

<script>
import StartScreen from '~/components/StartScreen.vue'
import AppBar from '~/components/AppBar.vue'
import FootBar from '~/components/FootBar.vue'
import Chats from '~/components/Chats.vue'

export default {
  components: {
    StartScreen,
    AppBar,
    FootBar,
    Chats
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

<style></style>
