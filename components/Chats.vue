<template>
  <div class="chats">
    <MessageCard
      v-for="message of messages"
      :message="message"
      :key="message.id"
    />
  </div>
</template>
<script>
import MessageCard from '~/components/MessageCard.vue'

export default {
  components: {
    MessageCard
  },
  data: () => ({
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
  })
}
</script>
<style scoped>
.chats {
  display: flex;
  flex-direction: column-reverse;
  max-height: 100vh;
  height: 100vh;
  overflow-y: scroll;
  max-width: 800px;
  width: 100%;
  background-color: #f4f4f4;
  padding-top: 10px;
  padding-bottom: 60px;
  margin: 0 auto;
  margin-top: 50px;
}
</style>
