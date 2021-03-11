<template>
  <div class="container">
    <div class="title">
      <span>👉🏻</span>
      <h1>Compre ou Venda</h1>
      <span>👈🏻</span>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.container {
  margin: 60px auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.title {
  display: flex;
  align-items: center;
  gap: 50px;
}

span {
  font-size: 30px;
}

h1 {
  font-size: 42px;
  color: var(--color);
}
</style>
