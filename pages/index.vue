<template>
  <div class="container">
    <div>
      <img :src="Avatar" alt="Eneh's Display Pix" class="avatar" />
      <h1 class="title">James, Eneh</h1>
    </div>
  </div>
</template>

<script>
import Avatar from '~/assets/avatar.png'

export default {
  components: {
    /* Logo */
  },
  data: () => ({
    Avatar
  })
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
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
  color: #fafcfd;
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
