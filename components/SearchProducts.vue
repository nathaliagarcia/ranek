<template>
  <div>
    <div class="search">
      <input type="text" placeholder="Digite aqui o que você procura..." />
    </div>
    <Button>Buscar 🔎</Button>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
div {
  width: 80%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 20px 0;
}

.search {
  background: linear-gradient(130deg, #a093ff 0%, #8876fd 100%);
  padding: 3px;
  border-radius: 25px;
  box-shadow: var(--shadow);
}

input {
  width: calc(100% - 50px);
  background: white;
  padding: 13px 25px;
  outline: none;
  border: none;
  border-radius: 25px;
}

button {
  margin-left: 15px;
}
</style>
