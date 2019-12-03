<template>
  <div class="container">
    <div v-if="isLoading">
      <img :src="Avatar" alt="Eneh's Display Pix" class="avatar" />
      <h1 class="title">James, Eneh</h1>
    </div>
    <form v-else>
      <img :src="Avatar" alt="Eneh's Display Pix" class="avatar" />
      <input type="text" placeholder="Your first name or nickname" />
      <button type="submit">meet james</button>
    </form>
  </div>
</template>
<script>
import Avatar from '~/assets/avatar.png'

export default {
  data: () => ({
    Avatar,
    isLoading: true
  }),
  methods: {
    loaded: function() {
      setTimeout(() => (this.isLoading = !this.isLoading), 4000)
    }
  },
  created: function() {
    this.loaded()
  }
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

div {
  width: 100%;
}

form {
  max-width: 600px;
  width: 90%;
  animation: unleash 5s;
}

input,
button {
  outline: none;
  border: none;
  padding: 1rem;
  max-width: 600px;
  width: 90%;
  color: #4265ed;
}
input {
  border-radius: 1rem;
  font-size: 2rem;
  margin: 30px 0;
  background-color: #e4f0f7;
  text-align: center;
}
button {
  border-radius: 2.5rem;
  font-size: 2.4rem;
  background-color: #e4f0e7;
  cursor: pointer;
  text-transform: capitalize;
  font-weight: bold;
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

@keyframes unleash {
  0% {
    transform: scale(0);
  }
  100% {
    transform: scale(1);
  }
}
</style>
