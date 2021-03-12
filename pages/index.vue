<template>
  <div class="container">
    <div class="title">
      <span>👍</span>
      <h1>Compre ou Venda</h1>
      <span>👎</span>
    </div>
    <SearchProducts />
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.container {
  margin: 80px auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.title {
  display: flex;
  align-items: center;
  gap: 40px;
}

span {
  font-size: 30px;
}

h1 {
  font-size: 52px;
  color: var(--purple);
}
</style>
