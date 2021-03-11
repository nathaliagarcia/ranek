<template>
  <header>
    <nav class="container">
      <n-link to="/" class="logo">
        <img src="@/assets/svg/ranek.svg" alt="Logo Ranek"
      /></n-link>
      <n-link to="/login" class="btn">Vender ✌🏻 Login</n-link>
    </nav>
  </header>
</template>

<script>
export default {}
</script>

<style scoped>
header {
  width: 100vw;
}

nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 25px 0;
}

img {
  width: 120px;
}

.btn {
  color: white;
  font-weight: bold;
  padding: 15px 30px;
  border: none;
  background: linear-gradient(130deg, #a093ff 0%, #8876fd 100%);
  border-radius: 25px;

  transition: all 0.25s;
}

.btn:hover {
  background: linear-gradient(50deg, #8876fd 0%, #a093ff 100%);
  transform: scale(1.05);
}
</style>
