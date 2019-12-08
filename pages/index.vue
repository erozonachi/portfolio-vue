<template>
  <StartScreen v-bind:startChatSession="startChatSession" v-if="!username" />
  <div v-else>
    <AppBar />
    <Chats :messages="messages" />
    <FootBar :sendMessage="sendMessage" />
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
    username: '',
    messages: [
      {
        id: 1,
        type: `sent`
      },
      {
        id: 2,
        type: `received`
      },
      {
        id: 3,
        type: `sent`
      },
      {
        id: 4,
        type: `received`
      },
      {
        id: 5,
        type: `sent`
      },
      {
        id: 6,
        type: `received`
      },
      {
        id: 7,
        type: `sent`
      },
      {
        id: 8,
        type: `received`
      },
      {
        id: 9,
        type: `sent`
      },
      {
        id: 10,
        type: `received`
      },
      {
        id: 11,
        type: `sent`
      },
      {
        id: 12,
        type: `received`
      }
    ]
  }),
  methods: {
    startChatSession: function(username) {
      this.username = username
    },
    stackMessage: function(message) {
      this.messages.unshift(message)
    },
    sendMessage: function(message) {
      this.stackMessage({
        id: this.messages.length + 1,
        type: 'sent',
        text: message
      })
    }
  }
}
</script>

<style></style>
