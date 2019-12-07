<template>
  <div class="navbar">
    <div class="container">
      <div class="user-info">
        <img :src="Avatar" alt="Eneh's Display Pix" class="avatar" />
        <h1 class="title">James</h1>
      </div>
      <div class="socials">
        <a target="_blank_" href="#"><span>L</span></a>
        <a target="_blank_" href="#"><span>G</span></a>
        <a target="_blank_" href="#"><span>T</span></a>
      </div>
    </div>
  </div>
</template>
<script>
import Avatar from '~/assets/avatar.png'

export default {
  data: () => ({
    Avatar
  }),
  props: {
    username: {
      type: String,
      required: true
    }
  }
}
</script>
<style scoped>
.navbar {
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed;
  top: 0px;
  width: 100%;
  height: 50px;
  background-color: #ffffff;
  border: none;
  border-bottom: 1px solid #f0f0f0;
  color: #4f4f4f;
}
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 800px;
  width: 100%;
  height: 50px;
  border-left: 1px solid #f0f0f0;
  border-right: 1px solid #f0f0f0;
}
.user-info {
  display: flex;
  justify-content: flex-start;
  align-items: center;
}
.avatar {
  width: 30px;
  border-radius: 50%;
  margin: 0 10px;
}
.title {
  font-size: 1.6rem;
  font-weight: bold;
  color: inherit;
  color: #4265ed;
}
.socials {
  display: flex;
  justify-content: flex-end;
  align-items: center;
}
.socials > a {
  text-decoration: none;
  color: inherit;
  margin-left: 10px;
}
a:visited {
  color: #4f4f4f;
}
a:link {
  color: #4f4f4f;
}
a:active {
  color: #4f4f4f;
}
a:last-of-type {
  margin-right: 10px;
}
</style>
