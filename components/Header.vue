<template>
  <header>
    <nav class="container">
      <n-link to="/" class="logo">
        <img src="@/assets/svg/ranek.svg" alt="Logo Ranek"
      /></n-link>
      <n-link to="/login">
        <Button>Vender ✌️ Login</Button>
      </n-link>
    </nav>
  </header>
</template>

<script>
export default {}
</script>

<style scoped>
header {
  width: 100vw;
  background: white;
  box-shadow: var(--shadow);
}

nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 23px 0;
}

img {
  width: 120px;
}
</style>
