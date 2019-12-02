<template>
  <div class="container">
    <div v-if="true">
      <img :src="Avatar" alt="Eneh's Display Pix" class="avatar" />
      <h1 class="title">James, Eneh</h1>
    </div>
    <div v-else>
      <form>
        <input type="text" placeholder="Your first name or nickname" />
        <button type="submit">Chat with James</button>
      </form>
    </div>
  </div>
</template>
<script>
import Avatar from '~/assets/avatar.png'

export default {
  data: () => ({
    Avatar
  })
}
</script>
<style scoped>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

input,
button {
  display: flex;
  outline: none;
  border: none;
  padding: 1rem;
  max-width: 800px;
  width: 90%;
  background-color: #e4f0f7;
  color: #4265ed;
}
input {
  border-radius: 1rem;
  font-size: 2rem;
  margin-bottom: 30px;
}
button {
  border-radius: 50%;
  font-size: 2.4rem;
}

.avatar {
  max-width: 200px;
  border-radius: 50%;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 400;
  font-size: 6.4rem;
  color: #e4f0f7;
  letter-spacing: 1px;
  animation: bounce-in 2.5s;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

@keyframes bounce-in {
  0% {
    transform: scale(0);
  }
  50% {
    transform: scale(1.25);
  }
  100% {
    transform: scale(1);
  }
}
</style>
