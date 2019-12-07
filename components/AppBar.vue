<template>
  <div class="navbar">
    <div class="container">
      <div class="user-info">
        <img :src="Avatar" alt="Eneh's Display Pix" class="avatar" />
        <h1 class="title">James, Eneh</h1>
      </div>
      <div class="social-handles">
        <a target="_blank_" href="#"><span></span></a>
        <a target="_blank_" href="#"><span></span></a>
        <a target="_blank_" href="#"><span></span></a>
      </div>
    </div>
  </div>
</template>
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
</style>
