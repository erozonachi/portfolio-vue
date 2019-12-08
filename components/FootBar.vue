<template>
  <div class="footbar">
    <div class="container">
      <button class="commands">···</button>
      <form>
        <input type="text" placeholder="Type message..." v-model="message" />
        <button type="submit">send</button>
      </form>
    </div>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      message: ''
    }
  }
}
</script>
<style scoped>
.footbar {
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed;
  bottom: 0px;
  width: 100%;
  height: 60px;
  background-color: #ffffff;
  border: none;
  color: #4f4f4f;
}
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 800px;
  width: 100%;
  height: 60px;
  border-left: 1px solid #f0f0f0;
  border-right: 1px solid #f0f0f0;
  border-top: 1px solid #f0f0f0;
}
.commands {
  border: none;
  outline: none;
  background-color: inherit;
  font-weight: bold;
  font-size: 2.8rem;
  color: #4265ed;
}
form {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 94%;
}
input,
button {
  outline: none;
  border: none;
  padding: 1rem;
}
input {
  border-radius: 1rem;
  font-size: 1.8rem;
  margin: 30px 0;
  background-color: #e4f0f7;
  width: 90%;
}
button {
  border-radius: 2rem;
  font-size: 1.8rem;
  background-color: inherit;
  color: #4265ed;
  cursor: pointer;
  text-transform: uppercase;
  font-weight: bold;
}
</style>
