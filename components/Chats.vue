<template>
  <div class="chats">
    <p>1. My name is James, Eneh; you're lookiing at my portfolio app...</p>
    <p>2. My name is James, Eneh; you're lookiing at my portfolio app...</p>
    <p>3. My name is James, Eneh; you're lookiing at my portfolio app...</p>
    <p>4. My name is James, Eneh; you're lookiing at my portfolio app...</p>
  </div>
</template>
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
  padding-top: 50px;
  padding-bottom: 60px;
  margin: 0 auto;
}
p {
  align-self: flex-end;
}
</style>
