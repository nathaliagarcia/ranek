<template>
  <div class="container">
    <div class="title">
      <span>👍</span>
      <h1>Compre ou Venda</h1>
      <span>👎</span>
    </div>
    <SearchProducts />
    <section v-if="products" class="products">
      <CardProduct
        v-for="product in products"
        :key="product.id"
        :product="product"
      />
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: {},
    }
  },

  created() {
    this.getProducts()
  },

  methods: {
    async getProducts() {
      const products = await this.$axios.$get('produtos')
      this.products = products
    },
  },
}
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

.products {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-start;
  gap: 20px;
}
</style>
