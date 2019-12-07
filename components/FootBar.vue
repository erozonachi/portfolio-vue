<template>
  <div class="footbar">
    <div class="container">
      <button class="commands">···</button>
      <form>
        <input type="text" />
        <button type="submit">send</button>
      </form>
    </div>
  </div>
</template>
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
  border-top: 1px solid #f0f0f0;
  color: #4f4f4f;
}
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 800px;
  width: 100%;
}
.commands {
  border: none;
  outline: none;
  background-color: inherit;
  font-weight: bold;
  font-size: 1.6rem;
}
</style>
