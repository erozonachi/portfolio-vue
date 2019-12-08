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
  props: {
    messages: {
      type: Array,
      required: true
    }
  }
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
