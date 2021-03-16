<template>
  <div class="card">
    <img :src="require('@/assets/images/' + product.fotos)" />
    <div class="content">
      <div class="infos">
        <h2>{{ product.nome }}</h2>
        <p>{{ product.descricao }}</p>
        <h3>{{ product.preco | floatToReal }}</h3>
      </div>
      <Button>🛒</Button>
    </div>
  </div>
</template>

<script>
export default {
  filters: {
    floatToReal(value) {
      const price = parseInt(value)
      return price.toLocaleString('pt-BR', {
        style: 'currency',
        currency: 'BRL',
      })
    },
  },

  props: {
    product: {
      type: Object,
      required: true,
    },
  },
}
</script>

<style scoped>
.card {
  width: 280px;
  background: white;
  border-radius: 25px;
  box-shadow: var(--shadow);
  transition: all 0.25s ease;
}

img {
  width: 280px;
  height: 300px;
  object-fit: cover;
  object-position: center;
  border-radius: 25px 25px 0 0;
}

.content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px 15px;
  gap: 5px;
}

button {
  font-size: 20px;
  padding: 12px;
  border-radius: 15px;
}

h2 {
  font-size: 28px;
  color: var(--purple);
}

p {
  color: var(--color);
  font-size: 14px;
  white-space: nowrap;
  width: 180px;
  overflow: hidden;
  text-overflow: ellipsis;
}

h3 {
  font-size: 28px;
  padding-top: 10px;
  color: var(--color);
}
</style>
