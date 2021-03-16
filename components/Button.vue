<template>
  <button>
    <slot></slot>
  </button>
</template>

<script>
export default {}
</script>

<style scoped>
button {
  color: white;
  font-weight: bold;
  padding: 15px 30px;
  border: none;
  background: linear-gradient(130deg, #a093ff 0%, #8876fd 100%);
  border-radius: 25px;
  cursor: pointer;
  outline: none;

  transition: all 0.25s;
}

button:hover {
  background: linear-gradient(50deg, #8876fd 0%, #a093ff 100%);
  transform: scale(1.05);
  box-shadow: var(--shadow);
}
</style>
