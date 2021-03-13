<template>
  <div>
    {{ product.nome }}
    <img src="../assets/images/notebook.jpg" />
  </div>
</template>

<script>
export default {
  props: {
    product: {
      type: Object,
      required: true,
    },
  },
}
</script>

<style></style>
