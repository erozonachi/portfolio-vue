<template>
  <p :class="message.type == `sent` ? `sent` : `received`">
    1. My name is James, Eneh; you're lookiing at my portfolio app...
  </p>
</template>
<script>
export default {
  props: {
    message: {
      type: Object,
      required: true
    }
  }
}
</script>
<style scoped>
.sent,
.received {
  display: flex;
  flex-direction: column;
  max-width: 300px;
  width: fit-content;
  border-radius: 5px;
  border: 1px solid #ffffff;
  padding: 10px;
  margin: 10px;
  color: #333333;
}
.sent {
  background-color: #e4f0f7;
  align-self: flex-end;
}
.received {
  background-color: #fafafa;
  align-self: flex-start;
}
</style>
